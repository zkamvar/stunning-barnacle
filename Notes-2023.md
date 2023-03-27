# Meeting Notes

## Table of Contents

 - [2023-03-25](#date-2023-03-25)
 - [2023-03-17](#date-2023-03-17)
 - [2023-03-10](#date-2023-03-10)
 - [2023-02-17](#date-2023-02-17)
 - [2023-02-09](#date-2023-02-09)
 - [2023-01-27](#date-2023-01-27)
 - [2023-01-20](#date-2023-01-20)
 - [2023-01-13](#date-2023-01-13)
 - [2023-01-06](#date-2023-01-06)

### Date: 2023-03-25

#### Who did you help this week?

 - Tim Dennis with updating styles and adding alt-text to some of the lc-r images
 - Maybe Kelly? I gave her access to the instructor training repo and explained
   why she did not actually need to delete her fork in the way that she was
   using it. 
 - Saba Ferdous by fixing our drat repository and providing her an explanation
   of why one of her processes failed
 - 

#### Who helped you this week?

 - Kevin Ushey by being super patient with me as I presented a super-sprawling
   bug report and working on the reproducible example
 - Rob by testing out the workflows permissions bug
 - Erin by discussion the strategy for the Maintainer onboarding. 

#### What did you achieve?

This week, my intention was to dig a bit into the lesson-transition script so
that I could confirm that it worked on other machines. In the process, I
realised that I was rapidly running out of space on my machine, so I spent a
little time purging ~30GB. In addition, I found a pretty significant bug from
{renv} > 0.16.0 that set me back a few days along with an unrelated recent
implementation of GitHub workflows permissions features that was documented,
but never implemented until last week. 

Here's a breakdown of what happened:

 - (lesson-transition) Update workflow and documentation for portability and reliability
   - [(lesson-transition) update README to point to resources and add warnings](https://github.com/carpentries/lesson-transition/commit/8d742f91b2f96a3d6d6be01406687c57b0ff4c20)
   - [add code to auto-remove submodules that are released/ignored](https://github.com/carpentries/lesson-transition/commit/c0a733870b46169c0de071b475c2267ded370129)
   - [add internal documentation for how submodules are provisioned/destroyed](https://github.com/carpentries/lesson-transition/commit/551575caed718b75de899ba2ff77587f09dfdc72)
 - [(lesson-transition) address problems bootstrapping from a clean slate with {renv}](https://github.com/carpentries/lesson-transition/issues/18)
   - [fix the files that {renv} sees so that it can auto detect needed packages](https://github.com/carpentries/lesson-transition/commit/a46fefb9fbeb994ce93c657f6a710cd5e98e76ce)
   - [{renv} discovered a bug in the CRAN version where already installed packages were being skipped during provisioning](https://github.com/rstudio/renv/issues/1177)
     - [spent a few hours to create a reproducible example](https://github.com/zkamvar/renv-issue-1177)
   - [{sandpaper} 0.11.13 update `manage_deps()` to workaround renv issue 1177](https://github.com/carpentries/sandpaper/pull/423)
   - [(actions) re-allow current {renv} with GitHub actions](https://github.com/carpentries/actions/pull/71)
   - [update the versions of {renv} and {sandpaper} to solve the {renv} issue](https://github.com/carpentries/lesson-transition/commit/dbd0ea9358c1a02dadaac29e66942e810d7e150b)
 - [{sandpaper} update workflows so that pull request previews and comments will work](https://github.com/carpentries/sandpaper/pull/421)
   - This [fixed an issue with _new_ repositories](https://github.com/carpentries/sandpaper/issues/420)
   - I forked a third-party action to our organisation for an extra layer of
     security: <https://github.com/carpentries/create-pull-request>. Now the
     only actions we use are from either us, GitHub, or Posit (aka RStudio aka
     r-lib).
   - [updated workflows for R Markdown template](https://github.com/carpentries/workbench-template-rmd/commits?author=zkamvar&since=2023-03-20&until=2023-03-25)
   - [updated workflows for Markdown template](https://github.com/carpentries/workbench-template-md/commits?author=zkamvar&since=2023-03-20&until=2023-03-25)
 - [(lesson-transition) write transition workflow for `lc-r`](https://github.com/carpentries/lesson-transition/issues/19)
   - Tim Dennis had requested help with continuous integration for the lc-r lesson, so I [updated styles](https://github.com/LibraryCarpentry/lc-r/pull/84)
   - I used this as opportunity to try the conversion script for this lesson
   - This was complicated because of a particular set of uncommon modifications to the lesson
 - [(datacarpentry/r-raster-vector-geospatial) fixed an accidental reversion of episode 3](https://github.com/carpentries/sandpaper/issues/411#issuecomment-1481197388)
 - [(carpentries/drat) added support for Big Sur MacOS](https://github.com/carpentries/drat/commit/0e60207161d816f377ade095bf4f432b1920bc5b)
 - Workbench: co-worked during the beta phase meeting to compose tweets for the May rollout

#### What did you struggle with?

Several high-priority bugs pulling me in different directions, preventing me
from making progress on my original goals

#### What would you like to work on next week

 - reach out to r ecoloy and librarycarpentry maintainers (from five weeks ago)
 - continue to organise transition script to make sure all of our lessons work
 - release new {tinkr} version to CRAN
 - for the future
   - work on {tinkr} updates to parse in-chunk options
   - work on code handout

#### Where do you need help from Toby?

Nowhere! You are on a well-deserved vacation! 

#### What did you learn this week?

A well-crafted reproducible example, even if it takes a few hours to formulate,
can produce really quick bugfixes. 

AND

The Workbench pull request previews work really well to detect weird situations
where a file is accidentally reverted. 

### Date: 2023-03-17

#### Who did you help this week?

 - Sarah Stevens by reviewing her positconf submission
 - James Foster by showing the migration of the SQL ecology lesson
 - Talisha by confirming her question about updating her feature branch
 - Rob by showing that we _do_ rely on some docker hub integrations
 - Karen by clarifying why Kelly was in "read purgatory" for instructor-training
   and gave her admin access
 - Jens Brinkmann by giving pointers about how to format markdown for python
   output
 - Saba Ferdous by walking her through the steps to update her fork of {sandpaper}
 - Danielle by pointing out a misspelled email link in her slack message

#### Who helped you this week?

 - Everyone by being supportive after JoMo's death. I'm really glad that I work in a place where this kind of significant pain is not brushed off because he wasn't human.
 - Erin by reviewing my dovetail blog post for contributor names
 - Toby by sharing his job plan and the onboarding survey results
 - Rob by postponing our meeting
 - Brynn by posting a talk from AXEcon about accessibility automation

#### What did you achieve?

This week was a bit unfocussed, but I do think I made enough progress.

 - [Published Dovetail number 16](https://carpentries.org/blog/2023/03/dovetail-16/), thanking the styles maintainers
 - [(maintainer-onboarding) transition to Workbench](https://github.com/carpentries/maintainer-onboarding/issues/69#issuecomment-1474284839)
 - [{sandpaper} fixed instructor view asset linking](https://github.com/carpentries/sandpaper/pull/409)
 - [{sandpaper} actually provision `learners/reference.md` for new lessons](https://github.com/carpentries/sandpaper/pull/412)
   - [propogate to markdown template](https://github.com/carpentries/workbench-template-md/pull/21)
   - [propogate to R markdown template](https://github.com/carpentries/workbench-template-rmd/pull/34)
 - [{sandpaper} identified and fixed a bug with renv 0.17.1](https://github.com/carpentries/sandpaper/pull/416)
 - [{varnish} update lab logo and fix some bugs (thanks toby!)](https://github.com/carpentries/varnish/pull/76)
 - [(lesson-transition) add sql-ecology-lesson](https://github.com/carpentries/lesson-transition/commit/7333e6ceda3ee18c25ef7bbfe6cf64c879782ce3)
   this involved fixing some edge cases for headings and empty files

#### What did you struggle with?

{renv} letting me down yet again. I mostly struggled with being able to focus on any given task.

#### What would you like to work on next week

 - reach out to r ecoloy and librarycarpentry maintainers (from four weeks ago)
 - organise transition script to make sure all of our lessons work
 - for the future
   - work on {tinkr} updates to parse in-chunk options
   - work on code handout

#### Where do you need help from Toby?

Nowhere atm, just cancel any meetings we don't need and take rest. 

#### What did you learn this week?

Not this week.

### Date: 2023-03-10

#### Who did you help this week?

 - I helped Maneesha, Toby, and Erin find out why it was not clear who was
   responsible for the Workshop Template repository (spoiler alert: it's was 
   under governance of the Lesson Infrastructure Committee)
 - I helped Brynn assign Maneesha as a reviewer on a pull request
 - I helped clarify to Karen about why she shouldn't delete the mailmap file
   quite just yet. 
 - I "helped" Kelly by giving her the background of the Matomo integration and
   suggesting that we use the decision-making framework to determine who should
   make the calls regarding it.
 - I showed Talisha the correct URL to review the privacy policy

#### Who helped you this week?

 - Kevin Ushey helped a lot with being patient as I submitted my four bug reports
   to {renv}.
 - Maneesha confirmed that the AMY-fication of the Workshop Website generation
   is indeed on the infrastructure backlog.
 - Sarah Brown helped me by identifying a bug in the instructor note linking of
   images
 - Julien Colomb helped me by opening documentation issues for {sandpaper}

#### What did you achieve?

Much of this week was spent catching up and struggling with the update to {renv},
which introduced several silent bugs. 

 - [Updated {sandpaper} to work with newer {renv}](https://github.com/carpentries/sandpaper/pull/405)
   - [{renv} issue about failures with non-CRAN packages](https://github.com/rstudio/renv/issues/1156)
   - [{renv} issue about a locked folder in the package cache](https://github.com/rstudio/renv/issues/1158)
   - [{renv} issue about warnings in init](https://github.com/rstudio/renv/issues/1160)
   - [{renv} issue about a failure in a _very_ specific R environment](https://github.com/rstudio/renv/issues/1161)
   - [(R-Universe) added {renv} patch so that people can upgrade without being burned](https://github.com/carpentries/universe/commit/ebb35946fc502273abaa30332b49b9905dc1cb68)
   - [(actions) temporarily force renv 0.16.0 until our universe version was available](https://github.com/carpentries/actions/commits?author=zkamvar&since=2023-03-06&until=2023-03-11)
   - [(zkamvar/vise) temprarily force renv 0.16.0 until universe version was available](https://github.com/zkamvar/vise/issues/4)
 - Re-triggered package cache updates for sandpaper-docs, r-socialsci, workbench-template-rmd, and r-raster-vector-geospatial
   - [Pull Request for r-raster-vector-geospatial resulted in changes that caused some errors in the lesson that were caught by the maintainer](https://github.com/datacarpentry/r-raster-vector-geospatial/pull/389)
 - [{sandpaper} labelled instructor notes issue as a bug](https://github.com/carpentries/sandpaper/issues/404)
 - [{sandpaper} identified pandoc identifier quirk](https://github.com/carpentries/sandpaper/issues/403)
 - [{varnish} addressed Sarah Brown's question about Mermaid.js](https://github.com/carpentries/sandpaper-docs/issues/130)
 - [(workbench-template-md) answered questions about broken glossary link and search bar](https://github.com/carpentries/workbench-template-md/issues/20)
 - [{sandpaper} reviewed pull request for updated CONTRIBUTING.md document](https://github.com/carpentries/sandpaper/pull/407)

There was also discussion about the export to etherpad mixed with exported
notes somewhere in there, but I can't find it right now.

#### What did you struggle with?

I struggled a lot with trying to juggle broken things from {renv} along with
needs from the community popping up, updating my Job Plan, planning
communications for The Beta Phase, writing the dovetail blog post, and
addressing the lesson transition process. It's been a long week. I still feel
very much like I'm in responsive mode and I think part of this is likely due to
the fact that we lost two Curriculum Team members in 2022 and have only
increased our workload inside and outside of the team.

#### What would you like to work on next week

 - reach out to r ecoloy and librarycarpentry maintainers (from three weeks ago)
 - organise transition script to make sure all of our lessons work
 - for the future
   - work on {tinkr} updates to parse in-chunk options
   - work on code handout

#### Where do you need help from Toby?

How should I categorise the Germany trip in the Job Plan? Is it General or
shoudl it go in its own Moore grant category or something? 

#### What did you learn this week?

It's important to be around for at least a week after a major release.

### Date: 2023-02-17

#### Who did you help this week?

 - I helped Angelique by providing a roadmap for the Glosario grant
 - I helped Maneesha by providing some context for the pull request issue templates
 - I helped Andy Rominger by providing context of what to do with data in a lesson
 - I helped Alycia by making a video visible
 - I helped Toby by pointing him to OpenPeeps
 - I helped Richard Ostler by providing context around acknowledging funders


#### Who helped you this week?

 - Maneesha told me her preference for the post-Germany meeting and I was able to book my train and hotel tickets
 - Erin helpe me by putting herself on the hook for the teaching duty
 - Jon Jablonski helped me by giving more context to a use pattern that will no longer exist with The Workbench (adding lesson episodes to workshop website repositories)
 - Alycia helped me by pointing to a question from the instructors meeting that I could answer
 - Toby helped me by providing time in the CurrT meeting to discuss what happens with maintainers and PRs during the transition.
 - Vini helped me by being super excited about The Workbench
 - Sher, Kelly, and Alycia helped me by offering to help out with my lab meeting that happens during my vacation


#### What did you achieve?

Much of this week was working on the transition workflow for four bioconductor
lessons. Overall it went very well with only one minor hiccup.

 - Update lesson-transition repository for production transitions: <https://github.com/carpentries/lesson-transition/commits?author=zkamvar&since=2023-02-13&until=2023-02-17>
   - [managing-computational-projects](https://github.com/carpentries-incubator/managing-computational-projects/issues/67) transition successful
   - [bioc-intro](https://github.com/carpentries-incubator/bioc-intro/issues/76) transition successful
   - [bioc-rnaseq](https://github.com/carpentries-incubator/bioc-rnaseq/issues/15) transition successful, execution delayed (due to ephemeral package update error)
   - [bioc-project](https://github.com/carpentries-incubator/bioc-project/issues/48) transition successful
 - [{sandpaper} allow blank or character timings to assume 5 minutes](https://github.com/carpentries/sandpaper/pull/396)
 - [{sandpaper} allow bioconductor packages to be provisioned](https://github.com/carpentries/sandpaper/pull/397)
 - [wrote up release workflow](https://github.com/carpentries/lesson-transition/blob/main/release-workflow.md)

#### What did you struggle with?

This week was similar to my previous work week: burn through everything to get
things out, but it wasn't that much of a struggle. 

#### What would you like to work on next week

 - reach out to r ecoloy and librarycarpentry maintainers
 - for the future
   - work on {tinkr} updates to parse in-chunk options
   - work on code handout

#### Where do you need help from Toby?

I'll see you in Deustchland

### Date: 2023-02-09

#### Who did you help this week?

 - I helped Alycia by providing details about CC-BY 4.0 vs 2.0
 - I attempted to provide assistance to a slightly confused community member who
   didn't know what to do with editing a lesson
 - I helped Sarah Kaspar and Mark Crowe debug a cache invalidation error in the
   package cache

#### Who helped you this week?

 - Toby helped me by sitting with me as I made the lesson releases
 - Karen helped me by sitting with me as I made the first transformation of a 
   beta phase lesson
 - Brynn helped me by walking through what her fork looked like after the beta
   stage transition
 - Maneesha helped me by providing assistance with the Google account
 - Sarah Brown helped me by pointing out a bad URL for the edit-this-page splash
   page.
 - Eli helped me by providing resources for accessibility testing
 - Danielle helpe me by providing context for arrival times for the CT retreat
 - Toby helped me by insisting I take a day off this week because of my overtime
 - Erin and Kelly helped me by reviewing my video
 - Alycia helped me by providing her blessing for me to upload videos to the 
   YouTube channel.

#### What did you achieve?

Hey look another long week, but I'm taking the day off tomorrow, so it's not
all bad. First and foremost, I have officially released four of the beta phase
lessons to the second stage and permanently transformed them to use The
Carpentries Workbench :tada:. In addition, I had to do a bit of debugging and a
lot of video editing.

 - released four lessons to use The Workbench: <https://github.com/carpentries/lesson-transition/commits?author=zkamvar&since=2023-02-06&until=2023-02-10>
   - this includes commit and ref maps so that people can look up what commits were discarded and what were changed
   - uploaded videos and created two new videos for The Carpentries Workbench Transition: <https://www.youtube.com/playlist?list=PLXLapl_LKb4eQ3xOFHpYEb15HF3-7cMPO>
   - fixed some boo boos related to the transition 
 - [{sandpaper} fixed bug where running `update_cache()` in a subfolder created a new `renv/` folder](https://github.com/carpentries/sandpaper/issues/391)
 - [(workbench documentation) updated a lot of documentation for the workbench](https://github.com/carpentries/workbench/commits?author=zkamvar&since=2023-02-06&until=2023-02-10)
 - [create dovetail number 15](https://github.com/carpentries/carpentries.org/pull/1582)

I'm sure there were other things, but hard to remember. The important thing is
that I accomplished what I said I would accomplish last week. 

#### What did you struggle with?

This week was similar to my previous work week: burn through everything to get
things out.

#### What would you like to work on next week

 - [transform managing-computation-projects incubator lesson](https://github.com/carpentries-incubator/managing-computational-projects/issues/67)
 - publish dovetail blog post
 - begin strategy for transforming lessons in 2.5 months
 - book Germany train and hotel tickets
 - write up reflection of release process
 - reach out to r ecoloy and librarycarpentry maintainers
 - for the future
   - work on {tinkr} updates to parse in-chunk options
   - work on code handout

#### Where do you need help from Toby?

Please look through the typeform responses from the Workbench open survey as a
feedback translator. 

### Date: 2023-01-27

#### Who did you help this week?

- I helped Toby by walking through the lesson release package with him and
  adding some additional documentation that will help clarify some of the
  nuanced features. 
- I helped Saba Ferdous by showing her how to update her fork of sandpaper and
  varnish and addressing a bug she was getting updating her lessons
- I helped Piotr by providing context for an AWS setting set up by François
  when he was testing out lesson deployment. 

#### Who helped you this week?

 - Karen Word, David PS, and Nathaniel Porter helped me by doing some relatively
   innocuous tests on the validation that surfaced some bugs that needed to be
   fixed.
 - Maëlle Salmon helped me by reviewing my pull request and making a coupld of
   quality-of-life fixes for {tinkr}
 - Toby helped me by working with me on the Astronomy lesson release and
   providing enough context that I was able to understand key modes of confusion
 - Toby helped me by adding the helpdesk times to the community calendar
 - Maneesha helped me by giving me access to a copy of the AWS Genomics password
   so that I could update it
 - Alycia helped me by reminding me about a community introduction call that I
   needed to prepare for
 - Erin helped clarify the status of TOR for next week

#### What did you achieve?

This week was a long week. I was working mostly on the beta phase transition and
providing updates to the infrastructure in response to both bug reports AND to
upstream changes in packages. I was able to record videos of the testing and 
confirm that the transition works well. 

 - [{sandpaper} created an update that will work for pandoc 3](https://github.com/carpentries/sandpaper/pull/385)
   - I also [got clarification of the appropriate method for dealing with this issue](https://github.com/jgm/pandoc-types/issues/91#issuecomment-1402685464)
 - [{sandpaper} fixed failing tests due to new {knitr} progress bars](https://github.com/carpentries/sandpaper/issues/389)
   - I even [had a toot about it](https://fosstodon.org/@zkamvar/109751846159823983)
 - [{sandpaper} fixed a bug where `learners/setup.md` was not provisioned if it wasn't specified](https://github.com/carpentries/sandpaper/pull/387)
 - [{sandpaper} reported bug about orphan RMarkdown documents causing failures](https://github.com/carpentries/sandpaper/issues/383)
 - [{sandpaper} reported bug about empty RMarkdown document causing failures](https://github.com/carpentries/sandpaper/issues/390)
 - [{pegboard} fixed and improved alt text validation](https://github.com/carpentries/pegboard/pull/108)
 - [{pegboard} fixed and improved link protocol validation](https://github.com/carpentries/pegboard/pull/109)
 - [{tinkr} fix mangling of relative link anchors](https://github.com/ropensci/tinkr/issues/85)
   - [(instructor training) give all maintainers unique IDs in README](https://github.com/carpentries/instructor-training/pull/1474)
 - [(workbench transition) wrote up strategy for creating notifications to forks](https://github.com/carpentries/lesson-transition/issues/14)
 - Created two videos for the Workbench Transition 
   - Video for maintainers: <https://youtu.be/MMTb3TNWAbo>
   - Video for contributors with forks: <https://youtu.be/FiroXXv9Eq0>
 - Attended community welcome session and answered questions
 - [(lesson release) created a whole bunch of fixes and documentation to the lesson release process](https://github.com/carpentries/chisel/commits?author=zkamvar&since=2022-12-04&until=2023-01-28)
   - helped with lesson releases for astronomy and four beta phase repos


#### What did you struggle with?

This week was not really a struggle week, it was more of a burn through
everything before I have to step away for a week week.

#### What would you like to work on next week

`s/next/in two/`

 - archive beta phase lessons
 - transition beta phase lessons
 - release beta phase lessons
 - upload videos
 - deal with fallout
 - update documentation for contributing to the workbench
 - for the future
   - work on {tinkr} updates to parse in-chunk options
   - work on code handout

#### Where do you need help from Toby?

Please audit the zenodo release files that I created against the lessons they
were created for. I only did a surface-level inspection, but I believe they
should be okay. I did not generate those for the R ecology lesson nor the
librarycarpentry shell lesson because we have had no response.

#### What did you learn this week?

Brittle tests are a pain in the ass.

### Date: 2023-01-20

#### Who did you help this week?

- I helped Eli by providing context for our Old Faithful etherpads going down at 02:00 every day.
- I took notes during the trainer meetings
- I helped the core team by having a hobbled Zoom during Toby's scavenger hunt
- I helped Sarah Stevens by providing context of where she should be suggesting changes
- I anti-helped Toby by giving him difficult jobs as my new supervisor

#### Who helped you this week?

- Alycia helped me by reminding me who Michael's supervisor was (to contact about CyVerse stuff)
- Agustina, Irene, and Kristi helped me by asking good questions during the maintainer meeting
- Members of the trainer community asked good questions during the trainer meeting
- Erin helped me by following up on some comments to clarify if some links were broken due to the workbench translation or due to another reason (it was both)
- Toby helped me make a decision regarding the unresponsive beta phase lessons
- Toby helped me by agreeing to email the non-responsive beta phase maintainers.

#### What did you achieve?

Most of my work this week was focussed on polishing the workflows for the beta
phase and coming up with concrete messenging for the maintainers and
contributors. The first day of the week was getting back to where I was from
last Friday's disaster (which wasn't all that bad). 

 - (beta phase) got [a rough video demoing the consequences of the transition](https://www.youtube.com/watch?v=angM-0eXHh8&amp;t=455s) uploaded
 - (beta phase) added a [detailed breakdown of the beta phase workflow](https://github.com/carpentries/lesson-transition/blob/main/beta-phase-workflow.md#beta-stage)
 - [(beta phase) created workflow that auto-closes Pull Requests to gh-pages branch](https://github.com/carpentries/sandpaper/issues/381)
 - [(beta phase) opened issue to auto-migrate standard file links](https://github.com/carpentries/lesson-transition/issues/12)
 - [(workbench) created a rudimentary docker container](https://github.com/carpentries/workbench/issues/39)
 - [(workbench) begin a FAQ (which sorely needs to be updated)](https://carpentries.github.io/workbench/faq.html)
 - [{sandpaper} found bug in Pandoc 3 that I must fix](https://github.com/carpentries/sandpaper/issues/380)
 - [{varnish} fix beta URL in footer and head](https://github.com/carpentries/varnish/pull/75)

#### What did you struggle with?

I often struggle a lot trying to make a concise video for messaging. It always
goes a bit pear shaped. 

#### What would you like to work on next week

It's actually the same as it was last week

 - prepare for lesson release of beta phase lessons
 - prepare for archiving of beta phase lessons
 - finalise beta phase transition plans and record video
 - plan the future of workbench helpdesk sessions
 - update documentation for contributing to the workbench
 - for the future
   - work on {tinkr} updates to parse in-chunk options
   - work on code handout

#### Where do you need help from Toby?

Nowhere I can think of, just patience

#### What did you learn this week?

Not sure :X

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
