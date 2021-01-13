# Rollout plan for the lesson template

The lesson template is split up into different modules, which can be user-tested
at different stages in the process.

## Main modules of the lesson template

Lesson Template --- source files

:   This refers to the folder structure and the configuration files that the maintainer will directly modify and interact with. The maintainer will use {sandpaper} to convert the lesson template into the lesson website.


Lesson Engine --- {sandpaper}

:   The controls of the lesson template. From here, the lesson maintainer is able to create, modify and deploy lessons. The main purpose for this component is to provide a validator for lessons and an engine that can render code inside a source file. While this uses all other components to build the lesson, they are all modular and can be replaced at any time as long as the all work in concert.


Lesson Style --- {varnish}

:   The underlying look and feel of the lesson website written in templated HTML, CSS, and JavaScript appropriate for the Static Site Generator. This lives separate from the lesson template and the lesson engine.

Lesson Template --- staging branch

:   The staging branch is an orphan git branch apart from the main branch that stages markdown files rendered from RMarkdown files so that inspecting the differences is easier for maintainers.

GitHub Actions --- workflow

:   This are workflow files that live in the `.github/workflows/` folder of the lesson template and should contain a series of modules that will automate lesson deployment. This can create staging branches and comment on pull requests to show contributors what changed in R-based lessons. This can be used independently of the new lesson template and only requires the concept of a staging branch (which most R-based lessons have). 


Package Cache --- workflow

:   This refers to the lockfile from {renv} that dictates the R environment used for rendering the episodes. This can be used independently of the lesson template.


## User Testing

Github Actions can be tested on R-based lessons. We can create a fork of one R-based core lesson and one R-based incubator lesson and work closely with the maintianers to test out the workflows. 


