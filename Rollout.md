---
title: Rollout plan for the lesson template
---

After several months of research and tooling, we are now at the conceptual
point where we can begin to roll out the new lesson template. Because the new
template will change how the community (Lesson Maintainers, Instructors, 
Learners) interact with the lessons, the goal of this document is threefold:

1. Identify the stakeholders
2. Identify the in(ter)dependent components of the new lesson template
3. Define a rough timeline for the rollout plan with measurable progress goals

This document will deal with components that the stakeholders will DIRECTLY
interact with, so aspects like versioning, static site generator engine, and
i18n will not be covered in this document. These are both covered in 
[The Landscape Document](index.html)

## Stakeholders

All Lesson Maintainers

:   These are the people who will be interacting with the lesson engine ({sandpaper}). At the basic level, they want a place to write markdown that will automatically turn to HTML when they push it to GitHub. 

Incubator Lesson Maintainers

:   These are maintainers who are in active development of lessons, so the will heavily use the lesson engine and the folder structure. The package cache may be a help or a hindrance to them if they are R maintainers. These maintainers will also be the first ones to be interested in testing out engines for notebook-based lessons. 


R Lesson Maintainers

:   These are lesson maintainers who have an additional requirement for their lessons: content is automatically generated on GitHub. These maintainers will interact with the GitHub Actions Pull Request workflows and staging branch.


Instructors

:   Have a stake in the Lesson Style and will interact with the lesson template source files when checking out. If they contribute to an R-based lesson, they will be interacting with the GitHub Actions Pull Request workflow.

Learners

:   Have a stake in the Lesson Style, but will not interact with the lesson template source files. This group will be one of the hardest to get feedback from because we don't have direct contact with them and they don't actively volunteer their time to helping The Carpentries. 

## Main modules of the lesson template

The current lesson template is a stand-alone enterprise that bundles all of the
tooling and styling needed to generate a lesson in the repository itself. The 
new template separates the tooling and styling from the lesson content (mostly).
Below are definitions of the modules that the above stakeholders would interact
with. These modules can be separated into two categories:

Interchangeable Modules

:   Modules that are packaged independent from one another and can be updated
    via version changes. These modules that will only work on the new 
    lesson template.

File Modules

:   Configuration or workflow files that live inside of the lesson template. 
    These control what software is used to generate lesson content and how the
    lesson should be built. All in this category are compatible with both the 
    old and new lesson templates. 

I have defined each module below and added notes about who will interact with
the modules (**Target**), what other modules this will interact with 
(**Works with**), and what modules each module depends on (**Depends**).

### Interchangeable Modules

Each of the modules listed here are standalone packages that can be updated 
independently of one another via version number. 

Lesson Structure

:   This refers to the folder structure and the configuration files that the
    maintainer will directly modify and interact with. The maintainer will use
    {sandpaper} to convert the lesson template into the lesson website.
    
    ::::::::::::::: info
    NOTE: technically, this is not a module, but it is important to test.
    ::::::::::::::::::::
    
    - **Target:** All Lesson Maintainers, Instructors
    - **Works with:** Lesson Engine
    - **Depends:** Lesson Engine

Lesson Engine --- [{sandpaper}](https://carpentries.github.io/sandpaper)

:   The controls of the lesson template. From here, the lesson maintainer is able to create, modify and deploy lessons. The main purpose for this component is to provide a validator for lessons and an engine that can render code inside a source file. While this uses all other components to build the lesson, they are all modular and can be replaced at any time as long as the all work in concert.
    
    - **Target:** All Lesson Maintainers
    - **Works with:** Lesson Structure, Lesson Validator
    - **Depends:** Lesson Structure

Lesson Validator --- [{pegboard}](https://carpentries.github.io/pegboard)

:   This is an R package that will replace `make check` in the current template.
    it will check the components of the Lesson Structure and the Episodes. This
    also serves as a translator between the old lesson template and the new
    template.
    
    - **Target:** All Lesson Maintainers
    - **Works with:** Lesson Engine
    - **Depends:** NA

Lesson Style --- [{varnish}](https://github.com/carpentries/varnish#readme)

:   The underlying look and feel of the lesson website written in templated HTML, CSS, and JavaScript appropriate for the Static Site Generator. This lives separate from the lesson template and the lesson engine.
    
    - **Target:** All Lesson Maintainers, Instructors, Learners
    - **Works with:** GitHub Actions, Lesson Engine
    - **Depends:** NA


### File Modules

Each of the modules listed here (with the exception of the staging branch) need
to be updated via a pull request changing the file. The GitHub Workflows are 
designed such that they use steps that are either defined in 
<https://github.com/marketplace/actions/> or 
<https://github.com/zkamvar/actions/>.

Staging Branch

:   The staging branch is an orphan git branch apart from the main branch that
    stages markdown files rendered from RMarkdown files so that inspecting the
    differences is easier for maintainers. NOTE: For the current Jekyll-based
    lessons, this branch is effectively the `gh-pages` branch since GitHub uses
    Jekyll on the backend to serve the site.
    
    - **Target:** R Lesson Maintainers, Instructors
    - **Works with:** Lesson Engine, GitHub Actions
    - **Depends:** NA

GitHub Workflow --- Deployment

:   GitHub workflow for deployment that uses three branches: development (main),
    staging (md-outputs), and deployment (gh-pages). The staging branch is only 
    required for R-based lessons or lessons that contain rendred content.
    NOTE: This is already a part of the workflow for R-based lessons (the 
    staging branch is `gh-pages` because GitHub is using Jekyll on the backend
    to serve the site. 
    
    - **Target:** All Lesson Maintainers
    - **Works with:** Lesson Engine, Staging Branch, Lesson Style
    - **Depends:** NA

GitHub Workflow --- Pull Request

:   GitHub workflow that can create staging branches and comment on pull
    requests to show contributors what changed in R-based lessons. This can be
    used independently of the new lesson template and only requires the concept
    of a staging branch (which most R-based lessons have). 
    
    - **Target:** R Lesson Maintainers, Instructors
    - **Works with:** Lesson Engine, Staging Branch
    - **Depends:** Staging Branch

GitHub Workflow --- CRON

:   Time-based workflows to update the package cache and rebuild the site using
    the latest version of the Lesson Engine and the Lesson Style. The package
    cache (for R-based lessons) comes in the form of an automated pull request
    that updates the `renv.lock` file once a quarter. The lesson page is rebuilt
    from the staging branch once a week with a new version of the Lesson Style.
    
    - **Target:** All Lesson Maintainers
    - **Works with:** Pull Request Workflow
    - **Depends:** Pull Request Workflow
  

Package Cache --- [{renv}](https://rstudio.github.io/renv/)

:   This refers to the lockfile from {renv} that dictates the R environment
    used for rendering the episodes. This can be used independently of the 
    lesson template and even GitHub Actions.
    
    - **Target:** R Lesson Maintainers
    - **Works with:** CRON Workflow
    - **Depends:** NA


## Rollout Plan

The rollout will involve three phases for each of the independent components: 
alpha, beta, and release.

::::::::::::::::::: info

This section is still under construction :weary:

I've realized that what I need to do is to first create the order in which the rollout should happen and THEN I can add them to the calendar. OH GOD JANUARY IS ALMOST OVER

::::::::::::::::::::::::



## Alpha Phase By Audience

### All Lesson Maintainers

### Incubator Lesson Maintainers

### R Lesson Maintainers

 1. GitHub Workflow --- Deployment
 2. GitHub Workflow --- Pull Requests

### Instructors

## Beta Phase By Audience

### All Lesson Maintainers

### Incubator Lesson Maintainers

### R Lesson Maintainers

### Instructors

### Learners

## Release By Audience

### All Lesson Maintainers

### Incubator Lesson Maintainers

### R Lesson Maintainers

### Instructors

### Learners

Github Workflow --- Deployment

:   Concept incoroporated into styles and deployed to R repositories using Jekyll lessons. (Françios will take care of this 4th week of January).


 - Figure out recruitment plan for target audiences.

 - Present on plan at CT meeting.


GitHub Workflow --- Pull Requests

:   1. (Zhian) Demonstration of concept in a fork of R-based repositories (incubator, swc, dc, and lc) with Jekyll architecture. Demonstrate pull requests in maintainer meeting.
    2. Ask people to test this on their own lessons
    3. Include incubator lesson.
     
    Feedback plan: ???
    Delivery plan: ???

Lesson Structure

:   1. (Zhian) Demonstrate lesson structure at the maintainer meeting.
    
    Feedback Plan: ???
    Delivery Plan: ???


