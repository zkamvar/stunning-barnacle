---
title: Rollout plan for the lesson template
---

The lesson template is split up into different modules, which can be user-tested
at different stages in the process.

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
    lesson template (with the exception of zkamvar/actions).

File Modules

:   Configuration or workflow files that live inside of the lesson template. 
    These control what software is used to generate lesson content and how the
    lesson should be built. All in this category are compatible with both the 
    old and new lesson templates. 

### Interchangeable Modules

Lesson Structure

:   This refers to the folder structure and the configuration files that the
    maintainer will directly modify and interact with. The maintainer will use
    {sandpaper} to convert the lesson template into the lesson website.
    
    ::::::::::::::: info
    NOTE: technically, this is not a module, but it is important to test.
    ::::::::::::::::::::
    
    - Target: All Lesson Maintainers, Instructors
    - Works with: Lesson Engine
    - Depends: Lesson Engine
    - Update: Pull Request

Lesson Engine --- [{sandpaper}](https://carpentries.github.io/sandpaper)

:   The controls of the lesson template. From here, the lesson maintainer is able to create, modify and deploy lessons. The main purpose for this component is to provide a validator for lessons and an engine that can render code inside a source file. While this uses all other components to build the lesson, they are all modular and can be replaced at any time as long as the all work in concert.
    
    - Target: All Lesson Maintainers
    - Works with: Lesson Structure, Lesson Validator
    - Depends: Lesson Structure
    - Update: version

Lesson Validator --- [{pegboard}](https://carpentries.github.io/pegboard)

:   This is an R package that will replace `make check` in the current template.
    it will check the components of the Lesson Structure and the Episodes. This
    also serves as a translator between the old lesson template and the new
    template.
    
    - Target: All Lesson Maintainers
    - Works with: Lesson Engine
    - Depends: NA
    - Update: version

Lesson Style --- [{varnish}](https://github.com/carpentries/varnish#readme)

:   The underlying look and feel of the lesson website written in templated HTML, CSS, and JavaScript appropriate for the Static Site Generator. This lives separate from the lesson template and the lesson engine.
    
    - Target: All Lesson Maintainers, Instructors, Learners
    - Works with: GitHub Actions, Lesson Engine
    - Depends: NA
    - Update: version

GitHub Actions --- [zkamvar/actions](https://github.com/zkamvar/actions#readme)

:   A collection of actions written in JavaScript for use with github workflows
    that live in the lessons.

    - Target: NA
    - Works with: GitHub Workflows
    - Depends: NA
    - Update: version

### File Modules

Staging Branch

:   The staging branch is an orphan git branch apart from the main branch that
    stages markdown files rendered from RMarkdown files so that inspecting the
    differences is easier for maintainers. NOTE: For the current Jekyll-based
    lessons, this branch is effectively the `gh-pages` branch since GitHub uses
    Jekyll on the backend to serve the site.
    
    - Target: R Lesson Maintainers, Instructors
    - Works with: Lesson Engine, GitHub Actions
    - Depends: NA
    - Update: NA

GitHub Workflow --- Deployment

:   GitHub workflow for deployment that uses three branches: development (main),
    staging (md-outputs), and deployment (gh-pages). The staging branch is only 
    required for R-based lessons or lessons that contain rendred content.
    NOTE: This is already a part of the workflow for R-based lessons (the 
    staging branch is `gh-pages` because GitHub is using Jekyll on the backend
    to serve the site. 
    
    - Target: All Lesson Maintainers
    - Works with: Lesson Engine, Staging Branch, Lesson Style
    - Depends: NA
    - Update: Pull Request

GitHub Workflow --- Pull Request

:   GitHub workflow that can create staging branches and comment on pull
    requests to show contributors what changed in R-based lessons. This can be
    used independently of the new lesson template and only requires the concept
    of a staging branch (which most R-based lessons have). 
    
    - Target: R Lesson Maintainers, Instructors
    - Works with: Lesson Engine, Staging Branch
    - Depends: Staging Branch
    - Update: Pull Request

GitHub Workflow --- CRON

:   Time-based workflows to update the package cache and rebuild the site using
    the latest version of the Lesson Engine and the Lesson Style. The package
    cache (for R-based lessons) comes in the form of an automated pull request
    that updates the `renv.lock` file once a quarter. The lesson page is rebuilt
    from the staging branch once a week with a new version of the Lesson Style.
    
    - Target: All Lesson Maintainers
    - Works with: Pull Request Workflow
    - Depends: Pull Request Workflow
    - Update: Pull Request
  

Package Cache --- [{renv}](https://rstudio.github.io/renv/)

:   This refers to the lockfile from {renv} that dictates the R environment
    used for rendering the episodes. This can be used independently of the 
    lesson template and even GitHub Actions.
    
    - Target: R Lesson Maintainers
    - Works with: CRON Workflow
    - Depends: NA
    - Update: Pull Request


## User Testing

Github Actions can be tested on R-based lessons. We can create a fork of one R-based core lesson and one R-based incubator lesson and work closely with the maintianers to test out the workflows. 


