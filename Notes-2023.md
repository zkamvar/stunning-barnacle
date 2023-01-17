# Meeting Notes

## Table of Contents

 - [2023-01-13](#date-2023-01-13)
 - [2023-01-06](#date-2023-01-06)

### Date: 2023-01-13

#### Who did you help this week?

 - I helped Sher! by providing an attempt at context for our airport location policy (though Maneesha hit the point more on the head)
 - I deleted a SPAM email and provided context for Karen
 - I provided context for a GitHub build failure email that Alycia was getting
 - I helped Rob debug his Jekyll setup for the main website
 - I helped Angelique by letting her know about the (non-)state of governance for Glosario and that the training for glosario editors may piggyback on the maintainer training.

#### Who helped you this week?

 - Kari and Sher! provided context of how I should submit an agenda item to the Core Team meetings
 - Karen and Alycia helped me understand some unexpected communications challenges maintainers and lesson developers might face
 - Kelly alerted us to a potential ethics issue with Posit partering with Palantir
 - Maneesha added me to the sysadmin email group and provided context for messages that I would be seeing.
 - Karen helped me by informing me about the fact that one early tester had an issue early on forking a lesson for teaching and later letting me know that it was Tracy, which provided enough context for me to see that there were extra steps needed (see [my comment on her commit](https://github.com/tracykteal/r-tidyverse-4-datasets/commit/8ddf11edba4daf8a403b4b7d4126142db14ac4fe#comments)), which lead me to add the instructions for forks in the dovetail blogpost. 


#### What did you achieve?

A lot of this week was spent mostly on The Workbench and the beta phase. There
were also a bunch of tasks that I worked on related to infrastructure. The last
day this week was focused on polishing the process for transitioning
repositories into the beta stage and I accidentally lost all my work :( I'll
try to list what I did accomplish hopefully.

 - [(workbench) opened issue to document how to respond to failing workflow](https://github.com/carpentries/workbench/issues/38)
 - [(workbench) opened issue to document how instructors can create forks to teach from](https://github.com/carpentries/workbench/issues/37)
 - [(workbench) added an integration test for lessons](https://github.com/zkamvar/workbench-integration-test)
 - [(workbench) begin updating documentation for contributors (e.g. those that wish to develop the tooling)](https://carpentries.github.io/workbench/contributor/)
   - [begin contributor guide for sandpaper](https://carpentries.github.io/workbench/contributor/sandpaper.html)
   - [{sandpaper} begin update documentation for `build_lesson()`](https://carpentries.github.io/sandpaper/reference/build_lesson.html)
   - [{sandpaper} update documentation for `ci_deploy()` and add concrete example](https://carpentries.github.io/sandpaper/reference/ci_deploy.html)
   - [{sandpaper} combine and update documentation for `ci_build_*()` functions](https://carpentries.github.io/sandpaper/reference/ci_build.html)
 - [(workbench docs) update example of alt text](https://github.com/carpentries/sandpaper-docs/commit/eedc6ee20c5b884d83674e8af0bb3daab20977c8)
 - [(workbench docs) fixed really old typo that was confusing to some](https://github.com/carpentries/sandpaper-docs/issues/121)
 - [{pegboard} release a minor update to fix some failing tests due to changes in lesson-example](https://github.com/carpentries/pegboard/pull/105)
 - [(beta phase) fix formatting issues with the instructor training lesson](https://github.com/carpentries/lesson-transition/commit/0e714d1a70e275724e0b93f1540ca134fa4a5746)
 - [(beta phase) work on simulating a lesson transition](https://github.com/carpentries/lesson-transition/commit/0e714d1a70e275724e0b93f1540ca134fa4a5746)
 - [(beta phase) added notes regarding lost work on branch protection](https://github.com/carpentries/lesson-transition/commit/c92d9dd2d6ffd0f1fce74e10c560f1bd79f6c767)
 - [(infrastructure) open issue to update our SSL renewal process](https://github.com/carpentries/carpentries-certificates/issues/9)
 - [(infrastructure) update workflow for our feeds](https://github.com/carpentries/feeds.carpentries.org/pull/74)

#### What did you struggle with?

Juggling the workflow for the beta phase. Testing out automated manipulation of
a lesson repository is a big challenge because we only get one shot at it
(though because I am renaming and locking branches instead of deleting them, it
should not be that big of an issue). 

The task was difficult because I was trying to run the test this way:

1. make a copy of `sgibson91/cross-stitch-carpentry` to `fishtree-attempt/znk-transition-test`
2. open a pull request from an existing branch (to demonstrate where existing pull requests go)
3. run the transition workflow, which involves the following steps
  1. create a submodule for the lesson to be transitioned
  2. make a local copy of the lesson, filter the styles commits, and transform the contents
  3. move and lock the old branches
  4. push and protect the new branches
  5. restrict the maintainers of the existing lesson

Every time I ran the test, I had to start from 1. Steps 1 and 2 are acheived in 
a single script and 3 is achieved with a make command, but after 3 is run, I 
end up with a new git module staged that I do not wish to be staged, so I have
to run `git restore --staged . && rm -rf fishtree-attempt/znk-transition-test beta/fishtree-attempt/znk-transition-test*` to undo it. 
The problem was that I also needed to commit my progress with the transition
script every time I did it. 

#### What would you like to work on next week

 - finalise beta phase transition plans and record video
 - plan the future of workbench helpdesk sessions
 - update documentation for contributing to the workbench
 - for the future
   - work on {tinkr} updates to parse in-chunk options
   - work on code handout

#### Where do you need help from Kari?

Nowhere yet :)

#### What did you learn this week?

I learned that you can still make mistakes after 10 years working almost daily
with a particular tool. 

### Date: 2023-01-06

#### Who did you help this week?

 - I helped Erin and Rob by [shrinking the size of Rob's head](https://github.com/carpentries/carpentries.org/pull/1563/commits/b895d83abf8625efc61c95bbd38aa80a9a158df5)
 - I helped Eric Lease Morgan by providing instructions for updating workbench components
 - I helped Alycia by posting the [workbench in 2 minutes](https://youtu.be/x7tETGpF3-4) youtube video and captions to our channel
 - I helped Alycia by sharing a twitter/mastodon crossposter (https://moa.party/)

#### Who helped you this week?

 - Alycia helped me by setting aside time to talk through the Workbench Communications Plan 
 - Jennifer Stubbs helped me by hosting a community discussion about The Carpentries Workbench
 - Karen helped me by pointing out that I have to wait for the etherpad time slider contents to load

#### What did you achieve?

The first part of this week was spent on catching up, infrastructure
maintenance, and changing passwords. I focused a good chunk of time on
workbench communication and fixed a long-standing bug in {pegboard} that
affected the transition process. Here's a breakdown:

 - I alerted the team to the severity of the LastPass breach and assigned asana
   tasks for folks to change their passwords.
 - Joined a community discussion lead by Jennifer Stubbs about The Workbench
   - Followed up to a reply to an email from January WRT [The HPC series of
     lessons](https://github.com/carpentries-incubator/hpc-intro/) clarifying
     that I would need time to develop additional functionality into The
     Workbench to accomodate their needs.
 - Met with Alycia to flesh out beta phase communication plan
 - [(docuementation) made several improvements to the documentation](https://github.com/carpentries/workbench/commits?author=zkamvar&since=2023-01-01&until=2023-01-07)
   - [added screenshots to transition guide](https://carpentries.github.io/workbench/transition-guide.html#for-instructors)
   - [added a glossary of terms](https://carpentries.github.io/workbench/reference.html#glossary)
   - added video in header
 - [{pegboard} fixed a silent bug from September that caused the lesson transition script to fail to translate some jekyll-specific links](https://github.com/carpentries/pegboard/issues/100)
   - [updated workflows to run every week to avoid future
     problems](https://github.com/carpentries/pegboard/pull/102/commits/e644ad765108988f239166cb0c60c8199e40fa7b)
     (analysis: when I made a [major update to the workflows in
     september](https://github.com/carpentries/pegboard/commit/7d1dbdcae0c7d1581fe02d2ff1c969e054be156a),
     I forgot to re-add the step to run every week, so while they ran for every
     pull request, they would no longer run every week, so I was not informed
     about the change.
 - [{pegboard} started on an update that would allow code handouts to be generated automatically](https://github.com/carpentries/pegboard/pull/101)
 - [{sandpaper} updated workflows to run every week](https://github.com/carpentries/sandpaper/pull/377)

#### What did you struggle with?

I struggled a bit with trying to figure out how to implement the code handout
stuff, not realising that there was a bug that I hadn't previously detected. 

#### What would you like to work on when you come back from vacation?

 - work on {tinkr} updates to parse in-chunk options
 - work on code handout
 - think about strategies for infrastructure secruity
 - plan the future of workbench helpdesk sessions
 - update documentation for contributing to the workbench

#### Where do you need help from Kari?

Nowhere yet :)

#### What did you learn this week?

I learned that a small mistake can hide out for a while sometimes.
