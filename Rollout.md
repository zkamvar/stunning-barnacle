# Rollout plan for the lesson template

The lesson template is split up into different modules, which can be user-tested
at different stages in the process.

## Stakeholders

Lesson Maintainers

:   These are the people who will be interacting with the lesson engine ({sandpaper}). At the basic level, they want a place to write markdown that will automatically turn to HTML when they push it to GitHub. 

Incubator Lesson Maintainers

:   These are maintainers who are in active development of lessons, so the will heavily use the lesson engine and the folder structure. The package cache may be a help or a hindrance to them if they are R maintainers. These maintainers will also be the first ones to be interested in testing out engines for notebook-based lessons. 


R Lesson Maintainers

:   These are lesson maintainers who have an additional requirement for their lessons: content is automatically generated on GitHub. These maintainers will interact with the GitHub Actions Pull Request workflows and staging branch.


Instructors

:   Have a stake in the Lesson Style and will interact with the lesson template source files when checking out. If they contribute to an R-based lesson, they will be interacting with the GitHub Actions Pull Request workflow.



## Main modules of the lesson template

Lesson Template --- source files

:   This refers to the folder structure and the configuration files that the maintainer will directly modify and interact with. The maintainer will use {sandpaper} to convert the lesson template into the lesson website.


Lesson Engine --- {sandpaper}

:   The controls of the lesson template. From here, the lesson maintainer is able to create, modify and deploy lessons. The main purpose for this component is to provide a validator for lessons and an engine that can render code inside a source file. While this uses all other components to build the lesson, they are all modular and can be replaced at any time as long as the all work in concert.


Lesson Style --- {varnish}

:   The underlying look and feel of the lesson website written in templated HTML, CSS, and JavaScript appropriate for the Static Site Generator. This lives separate from the lesson template and the lesson engine.

Lesson Template --- staging branch

:   The staging branch is an orphan git branch apart from the main branch that stages markdown files rendered from RMarkdown files so that inspecting the differences is easier for maintainers.

GitHub Actions --- Pull Request workflow

:   This are workflow files that live in the `.github/workflows/` folder of the lesson template and should contain a series of modules that will automate lesson deployment. This can create staging branches and comment on pull requests to show contributors what changed in R-based lessons. This can be used independently of the new lesson template and only requires the concept of a staging branch (which most R-based lessons have). 


Package Cache --- workflow

:   This refers to the lockfile from {renv} that dictates the R environment used for rendering the episodes. This can be used independently of the lesson template.


## User Testing

Github Actions can be tested on R-based lessons. We can create a fork of one R-based core lesson and one R-based incubator lesson and work closely with the maintianers to test out the workflows. 


