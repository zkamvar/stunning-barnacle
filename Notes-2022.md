# Meeting Notes

## Table of Contents

 - [2022-11-18](#date-2022-11-18)
 - [2022-11-10](#date-2022-11-10)
 - [2022-11-04](#date-2022-11-04)
 - [2022-10-28](#date-2022-10-28)
 - [2022-10-21](#date-2022-10-21)
 - [2022-10-14](#date-2022-10-14)
 - [2022-10-07](#date-2022-10-07)
 - [2022-09-30](#date-2022-09-30)
 - [2022-09-23](#date-2022-09-23)
 - [2022-09-16](#date-2022-09-16)
 - [2022-09-02](#date-2022-09-02)
 - [2022-08-26](#date-2022-08-26)
 - [2022-08-19](#date-2022-08-19)
 - [2022-08-12](#date-2022-08-12)
 - [2022-07-22](#date-2022-07-22)
 - [2022-07-15](#date-2022-07-15)
 - [2022-07-08](#date-2022-07-08)
 - [2022-07-01](#date-2022-07-01)
 - [2022-06-24](#date-2022-06-24)
 - [2022-06-10](#date-2022-06-10)
 - [2022-06-03](#date-2022-06-03)
 - [2022-05-27](#date-2022-05-27)
 - [2022-05-20](#date-2022-05-20)
 - [2022-05-13](#date-2022-05-13)
 - [2022-05-06](#date-2022-05-06)
 - [2022-04-29](#date-2022-04-29)
 - [2022-04-22](#date-2022-04-22)
 - [2022-04-15](#date-2022-04-15)
 - [2022-04-08](#date-2022-04-08)
 - [2022-03-25](#date-2022-03-25)
 - [2022-03-18](#date-2022-03-18)
 - [2022-02-25](#date-2022-02-25)
 - [2022-02-18](#date-2022-02-18)
 - [2022-02-11](#date-2022-02-11)
 - [2022-02-04](#date-2022-02-04)
 - [2022-01-28](#date-2022-01-28)
 - [2022-01-21](#date-2022-01-21)
 - [2022-01-14](#date-2022-01-14)
 - [2022-01-07](#date-2022-01-07)

### Date: 2022-11-18

#### Who did you help this week?

 - I added some context WRT Mastodon for some of our core team members
 - I volunteered to take notes during the CT meeting when the notetaker was away
 - I can not remember much after that

#### Who helped you this week?

 - Erin sat down with me and helped me out of my rut
 - Kari helped by asking Erin to sit down with me
 - Alycia, Erin, and Vini helped me by providing good feedback during the workbench planning meetings
 - Toby helped me by giving space during the Curriculum Team meeting to discuss future plans for the beta phase and how the curriculum team could be involved.
 - Alycia helped me by coworking for a bit on communications.

#### What did you achieve?

This was a bit of a short week because I had to cut out a half day on Thursday.
I spent a lot of time working on the beta phase transition and demonstrating
what that would look like in an example repository (see https://github.com/zkamvar/transition-cross-stitch-carpentry). 

There was a lot of strategerizing about the workbench beta phase. 

#### What did you struggle with?

I still struggled with communication, but not nearly as much as last week.

#### What would you like to work on next week?

 - demonstrate second stage of beta phase on my fork and record video of what that looks like
 - communicate to instructors about workbench beta phase

#### Where do you need help from Kari?

Unknonw

#### What did you learn this week?

It's okay to ask for help. 

### Date: 2022-11-10

#### Who did you help this week?

 - I helped Drake Asberry by providing alternatives for installing the workbench
 - I helped Alycia and re-upped the LibraryCarpentry and DataCarpentry websites so they would rebuild
 - I helped Renato Alves (kinda) by letting him know that we do not yet have a docker container for the lesson infrastructure yet, but we would.

#### Who helped you this week?

 - Alycia sent me a message checking in on the survey tool for the workbench beta phase and invited me to her coworking session with Kelly to discuss it.
 - Talisha helped me figure out how to turn off an Asana task that would keep popping up from a crusty old project.
 - Toby helped me come up with ideas for handling the lack of maintainer engagement.

#### What did you achieve?

I think I acheived burnout. This feeling of energy just draining from my
shoulders, draping itself across the back of my chair, and finally flopping
into a wet slap on the floor. It's not great.

I had a day and a half off this week. One day for a holiday and a half day for
sick time. I believe I finished my performance reivews on Monday and then the
rest of the week fixing up odds and ends.

 - [{sandpaper} update timing format for the syllabus](https://github.com/carpentries/sandpaper/pull/363) from `XX:YY` to `XXh YYm`
 - [{sandpaper} discovered that lessons with bioconductor components could not run](https://github.com/carpentries/sandpaper/issues/365) unless those components were explicitly added. 
   - [{renv} opened an issue about the bioconductor packages](https://github.com/rstudio/renv/issues/1110). This took me a while to track down and I'm not even sure what the solution is yet. 
 - [(workbench documentation) opened an issue regarding better installation isntructions for python folks](https://github.com/carpentries/sandpaper-docs/issues/115)
 - [{varnish} temporarily turn off matomo analytics for our lessons](https://github.com/carpentries/varnish/pull/67) until we can get a better idea of what we want to do with these analytics.
 - [(workbench beta) update the dates for the beta phase](https://github.com/carpentries/workbench/commits?author=zkamvar&since=2022-11-07&until=2022-11-11)
 - [(lesson-transition) add catch that allows librarycarpentry/lc-shell to run](https://github.com/carpentries/lesson-transition/commit/3113e1a6f2772eb411d0b5c8667f8daa4c21f460). This lesson was not running because it was built with an old version of styles that was incompatible with my parser.
 - [(workbench) added friction log from slack](https://github.com/carpentries/workbench/discussions/33)

#### What did you struggle with?

I think I'm struggling with burnout. I feel very frustrated that I am not
getting much engagement on The Workbench Beta Phase. This frustration really
boils down to the fact that I do not want to alienate our maintainers any more
than they already feel alienated. I don't know how to communicate the need for 
testing to the maintainers in a way that excites them and makes them _want_ to 
try this out. My communications on this have been terrible, even to this team.
Like, if we do not test this, then we will have just wasted a bunch of time on
the workbench beta phase and it goes to prove that my job is just as worthless
and I will soon be unemployed. Everything feels terrible because I'm going to
make big changes to the repositories with our without permission in April and if
people are not prepared for it, we will get a lot of alienation that leads to
attrition. 

The whole point of this beta phase is so that I can get feedback in a
real-world situation of how it feels to work on an official lesson with this 
setup. The more people that use this, the better, but I can not get confirmation
that anyone beyond the early adopters are using this. The testing I did in 2021
was the ALPHA test, which simply tested if the tool I wrote works AT ALL. It
never tested whether or not it was ready for production across the 100+ lessons
and maintainers that we host and I think I have failed in my communication of
that aspect. 

#### What would you like to work on next week?

 - demonstrate second stage of beta phase on my fork (it's been on the top of my "shit to do" list for the last four weeks)
 - communicate to instructors about workbench beta phase
 - trying not to cry

#### Where do you need help from Kari?

A better way to ask this question because I never know even where to start. I know I need help, but I never know how.

#### What did you learn this week?

Everything sucks

### Date: 2022-11-04

#### Who did you help this week?

 - I invited Talisha to the infrastructure channel so that she could invite us to planning
 - I was a sounding board for Toby trying to figure out curriculum onboarding
 - I helped Nelly Selem (maintainer of r-novice-gapminder-es) with actually getting her on the repo and fixing a complex bug
 - I helped Michael by confirming that I got notified in an issue he opened
 - I added Maneesha to the Netlify account

#### Who helped you this week?

 - Alycia helped me multiple times by offering to help out with assessment for the beta phase (I never followed up `-_-`)
 - Alycia helped me by providing grounding words of context when I was gettin' panicky today about the lackluster response from maintainers
 - Eric Lease Morgan helped me by sending me a nearly complete friction log about setting up a lesson
 - Sarah Brown helped me by answering Eric Lease Morgan's question pretty much the way I would have


#### What did you achieve?

Hard to remember what happened this week, but I recall cancelling the Workbench
Beta Phase meeting because I was not prepared for it. In general, I fixed some
things and made some progress in documenting steps for the beta stage.

Here's what happened this week:

 - [I published dovetail number 10](https://carpentries.org/blog/2022/11/dovetail-010/)
 - I addressed a series of bugs related to workflow deprecations and errors.
   - [{sandpaper} update workflows to fix deprecations and use single branch for updates](https://github.com/carpentries/sandpaper/pull/356)
   - [(actions) update versions and avoid deprecations](https://github.com/carpentries/actions/pull/66)
   - [{vise} update to avoid deprecations](https://github.com/zkamvar/vise/pull/3). Testing this, I discovered and fixed another bug.
 - [(workbench docs) Updated the pull request documentation and screenshots](https://github.com/carpentries/sandpaper-docs/pull/113)
 - [(workbench beta phase) Updated documentation for updating repos after beta](https://carpentries.github.io/workbench/beta-phase.html#beta)
 - [(workbench beta phase) fixed issue with filtering commits and started work on beta workflow](https://github.com/carpentries/lesson-transition/commits?author=zkamvar&since=2022-10-31&until=2022-11-05)
 - [{varnish} fixed bug with footer](https://github.com/carpentries/varnish/issues/65)
 - [(r-novice-gapminder-es) updated styles to fix a lesson that was not building for the last two years :grimacing:](https://github.com/swcarpentry/r-novice-gapminder-es/pull/132) - Show Toby how to run the lesson release script
 - Send reminders about the beta phase to the maintainers
   - [R Ecology Lesson (unresponsive)](https://github.com/datacarpentry/R-ecology-lesson/discussions/799#discussioncomment-4059975)
   - [R Socialsci (semi-responsive)](https://github.com/datacarpentry/r-socialsci/discussions/411#discussioncomment-4061142)
   - [R geospatial (responsive)](https://github.com/datacarpentry/r-raster-vector-geospatial/issues/369#issuecomment-1304327777)
   - [Reminded OpenRefine-ecology maintainers about transition next week](https://github.com/datacarpentry/OpenRefine-ecology-lesson/discussions/275#discussioncomment-4058542)
   - [Reminded lc-shell maintainers about transition in two weeks](https://github.com/LibraryCarpentry/lc-shell/discussions/211#discussioncomment-4061104)

#### What did you struggle with?

I struggled a lot with trying to communicate with maintainers about the beta
phase. I felt like the maintainers have not had the time or capacity to play
around with the snapshot repositories before I migrate their default
repositories. I've told the maintainers that we can delay if they are not ready
for the transition, but so far I've gotten mostly silence. The thing I'm torn
about is the fact that they might not even have the capacity to tell me that
they do not have the capacity to work on the lesson. In general, management of
this project has been quite a bit of a struggle and I haven't even yet
communicated to the instructors about the beta phase. 

#### What would you like to work on next week?

 - demonstrate second stage of beta phase on my fork (it's been on the top of my "shit to do" list for the last three weeks)
 - communicate to instructors about workbench beta phase

#### Where do you need help from Kari?

A better way to ask this question because I never know even where to start. I know I need help, but I never know how.

#### What did you learn this week?

I learned that we need to do better for our i18n community.

### Date: 2022-10-28

#### Who did you help this week?

 - I helped Toby by showing him how to review a pull request for The Workbench and started a [contribution guide](https://carpentries.github.io/workbench/contributor/)
 - I didn't really help anyone else this week.

#### Who helped you this week?

 - A lot of people. I needed a lot of help this week and it's difficult to remember who did what.
 - Karen helped me by talking through my communication plan for [carpentries/styles#641](https://github.com/carpentries/styles/issues/641).
 - Omar helped me by outlining the steps I needed to take for the above.

#### What did you achieve?

I don't have much to say about this week other than it was exhausting.

Here's what happened this week:

 - [(workbench beta phase) I added a landing page for anyone who tries to edit a lesson in beta](https://github.com/carpentries/workbench/discussions/30#discussioncomment-3955501)
 - [(workbench beta phase) set up transition repository option to not filter git commit messages](https://github.com/carpentries/lesson-transition/commit/b85d0569f4b4e10feab479bfa890df2e2fa8cead)
 - [(workbench beta phase) add filters that will fix headings to make sure that they apporach uniformity](https://github.com/carpentries/lesson-transition/commit/c6f3882ef769b3f7a45835006f7311b8027332e2)
 - [(workbench beta phase) add the official beta phase repos to the lesson-transition repository](https://github.com/carpentries/lesson-transition/commit/82d4f872875a5248be62f95946cb408ceb12d4ae)
 - [datacarpentry/r-raster-vector-geospatial added pull request that fixes changed data structures](https://github.com/datacarpentry/r-raster-vector-geospatial/pull/378)
 - [rerun bug fixing workflow to catch lessons that had only one workflow file present](https://github.com/zkamvar/2022-10-20-workflow-bug/commits?author=zkamvar&since=2022-10-24&until=2022-10-29)
 - published dovetail number 9
 - started dovetail number 10
 - [forked and added documentation to the release script](https://github.com/fmichonneau/chisel/compare/main...carpentries:chisel:main)
 - tested lesson release script
 - wrote most of my performance review
 - released (and then delayed) R-socialsci into pre-beta stage

#### What did you struggle with?

Literally everything. Every single dang day is a struggle right now. 

#### What would you like to work on next week?

 - demonstrate second stage of beta phase on my fork

#### Where do you need help from Kari?

Nothing at the moment. 

#### What did you learn this week?

I learned the importance of mindset when creating scripts and room for deep work.
Back in July, when we were shown the lesson release process, the script came
with the caveat that it was not really well documented as it was not really
meant for public consumption given the sensitive nature of some of the data
going into the process. At the end of this week, I had to step through it and
reason about what the heck was going on. Some things that were difficult were
functions that were written and then superseded, API tokens that were expected
to be in the environment, data files that were expected, but only stored locally,
and fluid representations with variable names.

The reason I think it is important to keep mindset in mind when creating scripts
is that these things that I encountered could have been avoided if two things
were true: if the author had enough time dedicated to deep work and if they had
written this with the objective of allowing other people to use it. Because the
scope of the task was limited to once every few months, the script was written
as a one-off to only be used by one person. The thing is, it is easy to develop
in this kind of pattern, but it makes things harder down stream (even for 
yourself) when someone else (e.g. yourself in the future) tries to reproduce
the results on a different machine. I think it is important for me to keep things
like this in mind when I am developing my tools so that if I happen to leave,
the amount of frustration experienced going through my old scripts is minimal.

### Date: 2022-10-21

#### Who did you help this week?

 - I helped Toby by reviewing his slides for the CT meeting
 - I _think_ I helped Maneesha by trying to explain what the a maintainer query in redash was for
 - I helped Karen by answering a question about the beta phase

#### Who helped you this week?

 - Maneesha helped me by being super cool and understanding when I had verbal vomit in our slack chat
 - Maneesha also helped me by reminding me that our AWS training was being recorded so I didn't have to miss it due to fixing styles
 - Erin helped me by talking with me after the workbench beta phase meeting
 - Sher! helped me by providing an update on the workbench beta phase project from the WAT

#### What did you achieve?

The beginning of this week was a bit of a dumpster fire, but things got better.
Funny enough, I spent a lot of time fixing a problem that propogated to all of
our lessons that was exacerbated by the way we have styles set up. It's a great
example of the kinds of things that can go wrong with controlling a distributed
set of lessons and the extra maneouvers that have to be performed when updating
them in a way that prevents merge conflicts in the future. 

Here's what happened this week:

 - Release [pre-beta stage of R-ecology-lesson](https://github.com/datacarpentry/R-ecology-lesson/pull/819) :tada:
 - [addressed a question about the beta phase](https://github.com/carpentries/workbench/discussions/30)
 - [Submit dovetail number 9](https://github.com/carpentries/carpentries.org/pull/1498)
 - [(lesson-transition) created and tested pre-beta workflow](https://github.com/carpentries/lesson-transition/commits?author=zkamvar&since=2022-10-17&until=2022-10-22)
 - [(workbench site) begin contributions page for developers](https://github.com/carpentries/workbench/commits?author=zkamvar&since=2022-10-17&until=2022-10-22)
 - [Reviewed Maneesha's PR in feeds.carpentries.org](https://github.com/carpentries/feeds.carpentries.org/pull/66) that modifed the workflows for the instructor selection project.
 - [Reviewed Maneesha's PR for the maintainer profile page](https://github.com/carpentries/carpentries.org/pull/1501) that added the alumni page
 - [Fix workflow bug in R Ecology Lesson](https://github.com/datacarpentry/R-ecology-lesson/issues/822)
 - [addressed carpentries/styles#641](https://github.com/carpentries/styles/issues/641)
   - [fixed workflows in carpentries/styles](https://github.com/carpentries/styles/pull/643)
   - [created workflow to broadcast pull requests with styles patch](https://github.com/zkamvar/2022-10-20-workflow-bug/tree/documentation#readme)

#### What did you struggle with?

I struggled on Monday heavily because of the fear of messing something up during
the conversion of the lessons combined with the fact that I did not yet have the
pre-beta workflow written. I was able to get it written and I tested it for the
release on Monday, and Erin reminded me that the worst that can happen is really
not that bad. 

#### What would you like to work on next week?

 - demonstrate second stage of beta phase on my fork
 - add beta phase redirect page to varnish and styles

#### Where do you need help from Kari?

Nothing at the moment. 

#### What did you learn this week?

I learned that it _is_ possible to apply an individual patch to a downstream
repository without doing a full merge or cherry-picking. Applying a patch is
weird, but it works (most of the time). Moreover, now that I have that script,
I now have a better understanding of the state of our lessons (e.g. several 
official lessons have not had their styles updated since before I started).

#### Any other topics

The issue that I encountered with our lessons this week is actually something
that _could_ feasibly happen with the workbench. The only difference is that 
with The Workbench, I would not need to do a weird dance of trying to apply a
patch, I should be able to run a single command on the repository URLs to get
the pull requests to trigger. The thing about the workbench is that, because we
check for updates to the workflows every week, it's much less likely that a
lesson will be so far out of date. 

### Date: 2022-10-14

#### Who did you help this week?

 - I helped myself by recognising when I was incredibly anxious and taking time off for that

#### Who helped you this week?

 - Brynn helped me by prioiritizing the lessons entering into the beta stage for the accessibility checks

#### What did you achieve?

This week was an even shorter week than last week. I effectively worked 2.5
days, but I was definitely not at my best. I am a big fan of public
transportation, but I accidentally boarded the struggle bus to struggle town
this week and let me tell you: service there is infrequent and unreliable.

Here's what happened this week:

 - I sat on three interviews for the IT developer position
 - I met with Tom Mock, Tracy Teal, and Erin about potential RStudio funding for embedding Quarto into the workbench
 - [{sandpaper} opened an issue for single-branch updates](https://github.com/carpentries/sandpaper/issues/350)
 - [{sandpaper} opened an issue for considering treatment of "break" episodes](https://github.com/carpentries/sandpaper/issues/351)
 - [(actions) opened an issue to update actions to node16](https://github.com/carpentries/actions/issues/60)
 - [(actions) opened an issue to modify set-output commands](https://github.com/carpentries/actions/issues/61)
 - [Beta Phase: moved lesson-transition tool to carpentries organisation](https://github.com/carpentries/lesson-transition) and am now enforcing signed commits
 - [Beta Phase: (lesson-transition) I added a mechansism to the Makefile to allow me to continue destructive tests for the lessons not yet in beta while preserving lessons that are in beta.](https://github.com/carpentries/lesson-transition/commit/48132e042e60d9d3751506019e7599901ca96ca8) 
 - [Beta Phase: {varnish} add survey URL for beta phase feedback](https://github.com/carpentries/varnish/pull/62)
 - [Beta Phase: prepare R-ecology-lesson for beta phase](https://github.com/datacarpentry/R-ecology-lesson/pull/819)
 - [{gitcellar} opened pull request to allow subset of repositories to be archived](https://github.com/ropensci-org/gitcellar/pull/13)
 - I rotated the keys for [The Carpentries Apprentice](https://github.com/carpentries-app)
 - I helped a little bit with adding to the Maintainer handbook for the website.

#### What did you struggle with?

I struggled with a lot of things. I think the next time I go down to California,
I will need to make sure I have a day to buffer myself against the effects of
the transition between states of being. My anxiety was already high when I met
with RStudio about the Quarto funding and it made the experience less than great
because anxiety breeds paranoia. Unfortunately, everything seemed to catch up
with me on Thursday. In the morning, during the meetings, I could feel this
bubble of anxiety expanding from within my lungs and leeching its poison into
my veins as I sat with my skin tingling as if a thousand tiny ghosts were
walking up and down my arms with velcro shoes. I did recognise it early enough
for me to take the rest of the day off, but it is something I will have to
watch out for again. 

#### What would you like to work on next week?

 - release R-ecology-lesson to beta phase
 - write dovetail blog post
 - refine beta phase workflow for the transition repo
 - demonstrate second stage of beta phase on my fork

#### Where do you need help from Kari?

Hard to tell, but nowhere at the moment. 

#### What did you learn this week?

We apparently get 6 days of sick time that can be allotted towards caring for a
family member (though the allotment of sick time that we have already earned for
a particular type of time off seems a bit intrusive).

#### Any other topics

Not at the moment

### Date: 2022-10-07

#### Who did you help this week?

 - I helped Maneesha by sitting down with her on Monday and going through her plans for the new instructor badging strategy.
 - I helped Kari by uploading a photo of a new EC member to the site.
 - I helped Danielle by alerting her to a discrepancy of dates in an upcoming workshop.

#### Who helped you this week?

 - Maneesha helped me by showing me that our methods of organisation and thinking are very much alike and compatible
 - Alycia and Toby helped me by offering their zoom rooms for recording when mine was busted
 - Alycia, Erin, and Karen helped me by sitting in the first Workbench Beta Phase meeting and coming up with good ideas even though I was super not in a great frame of mind.
 - Alycia and Kelly helped me by taking time during their coworking session to help out with the Beta Phase of the workbench. 
 - Toby and Alycia helped me by reviewing my Dovetail Blog Post

#### What did you achieve?

This week was a short week for me because I was out Thursday helping my brother around the house.
I was able to accomplish a bit in terms of the beta phase as in I have officially announced the dates and met up with the CT members who could help.
All this was on top of a fun surprise that I got on Tuesday when I found a bug in {renv}.
Next week is going to be a shorter week (3 days), but there is a lot packed in those three days. 
Here's a breakdown (in no particular order):

 - [Announced Beta Phase dates in Dovetail number 8](https://carpentries.org/blog/2022/10/dovetail-008/)
 - [Made the decision to update the beta phase URL to https://preview.carpentries.org](https://github.com/carpentries/carpentries.org/pull/1492)
 - I recorded a quick video demonstrating what to expect in the beta phase of the workbench
 - I met with my workbench beta core team comrades
 - I updated my responsibilities to the curriculum team
 - [added https://preview.carpentries.org to our subdomains](https://github.com/carpentries/carpentries.org/pull/1492)
 - [(data-lessons/lesson-transition) updated transition script to make filtering easier; updated R-ecology-lesson script](https://github.com/data-lessons/lesson-transition/commits?author=zkamvar&since=2022-10-03&until=2022-10-08)
 - Tested deploy of two upcoming Beta lessons: <https://preview.carpentries.org/R-ecology-lesson> and <https://preview.carpentries.org/r-socialsci>
 - [Notified maintainers of lessons in beta about the time for their lesson entry](https://carpentries.github.io/workbench/beta-phase.html#timeline-lessons-entered-into-workbench-beta) (links in table lead to discussions)
 - [{renv} opened an issue detailing a new bug](https://github.com/rstudio/renv/issues/1088) and the following: 
   - [fixed workbench-template-rmd](https://github.com/carpentries/workbench-template-rmd/commits?author=zkamvar&since=2022-10-03&until=2022-10-08)
   - [fixed r-tidyverse-4-datasets PR in incubator](https://github.com/rstudio/renv/issues/1088)
   - [fixed new R-ecology-lesson PR in incubator](https://github.com/carpentries-incubator/R-ecology-lesson/pull/18#issuecomment-1268615243)
   - [{sandpaper} released 0.10.2 to remove AWS workflow and add renv/sandbox to .gitignore](https://github.com/carpentries/sandpaper/pull/343)
   - [{sandpaper} released 0.10.4 to fix a bug in 0.10.2 which caused all lessons built before 2022-10-04 to be invalid](https://github.com/carpentries/sandpaper/pull/348)
   - [(actions) update-lockfile action now inserts renv/sandbox into .gitignore](https://github.com/carpentries/actions/releases/tag/v0.12.2)
 - [{sandpaper} released 0.10.3 to remove an extra file introduced in 0.8.0 that was causing renv workflows to run every week](https://github.com/carpentries/sandpaper/pull/346)
 - [(carpentries/styles) opened PR to update workbench beta phase workflows and variables](https://github.com/carpentries/styles/pull/639)
 - [{varnish} released 0.2.5 to update the workbench banner](https://github.com/carpentries/varnish/pull/61)

#### What did you struggle with?

I struggled a lot with trying to figure out how to record the workbench beta
video. I was trying to use OBS studio and then realised that it's only for
recording videos and that you have to edit them in another program and tried
blender and rage quit. I ended up recording it in Zoom and it's good enough!

#### What would you like to work on next week?

 - merge styles pr for beta phase
 - come up with beta phase workflow for the transition repo
 - demonstrate second stage of beta phase on my fork

#### Where do you need help from Kari?

Nothing :)

#### What did you learn this week?

I learned this cool trick where you can make little rounded highlights around
text by adding `background: #FFC700; border-radius: 5px` to a span element:
<https://jsfiddle.net/329ycpst/>


#### Any other topics

Nope.

### Date: 2022-09-30

#### Who did you help this week?

 - I helped Maneesha and my future self by taking notes during our 30 minute consulting session with Backbone Consulting
 - I helped Maneesha by adding her new SSH key to our servers

#### Who helped you this week?

 - Toby, Yanina, and Erin helped my by reviewing my R Consortium proposal
 - Erin helped me understand how I can frame the scope of funding I could request
 - Alycia helped me by inviting me to the Community Development Team meeting to help determine a strategy for The Workbench beta phase
 - Alycia and Kelly helped me by working with me on a plan for Beta Phase assessment
 - Yanina helped me by talking with me about the scope of my R Consortium Grant Proposal
 - Sara Morsy helped me by confirming that an update to sandpaper worked

#### What did you achieve?

This week was like camping in drag: pretty intense. We had the reading and
reflection day during which I had written a 3000 word blog post about Kari's
prompt for me to think about Professional Development and growth. I was also
writing the R Consortium Grant proposal and planning aspects of the Beta Phase.
Here is a breakdown:

 - [Finished and submitted the proposal for the R Consortium ISC grant](https://github.com/zkamvar/isc-proposal-workbench-2022)
 - [{sandpaper} added support for a custom index title](https://github.com/carpentries/sandpaper/pull/342)
 - [(workbench site) added Beta Phase Page](https://carpentries.github.io/workbench/beta-phase.html)
 - Created three channels for the Beta Phase in Topicbox: workbench, workbench-beta-maintainers, workbench-beta-instructors
 - Worked with Alycia and Kelly to come up with a plan for evaluation
 - Emailed maintainers of the Workbench Beta Phase with the proposed schedule
 - [Proposed a timeline for the Beta Phase](https://carpentries.github.io/workbench/beta-phase.html#timeline-lessons-entered-into-workbench-beta)
 - [Wrote a 3,000 word blog post on Professional Development](https://zkamvar.netlify.app/blog/happy-cycling/) (note for Kari: there's a lot of backstory, so if you want to skip to the actual goals, head over to the [Ready Let's Go section](https://zkamvar.netlify.app/blog/happy-cycling/#ready-lets-go))
 - Scheduled a call with Tom Mock from Posit in mid-October about potential funding for Quarto work

#### What did you struggle with?

I actually did not struggle that much this week. Talking with my therapist last week and the feedback that I got from the proposal really boosted me.

#### What would you like to work on next week?

 - Transfer data-lessons/lesson-transtion to the carpentries organisation and work on a new conversion.

#### Where do you need help from Kari?

Nothing :)

#### What did you learn this week?

I learned that I can actually write grants if I have a fully-formed idea and I put my mind to it.

#### Any other topics

I made a [terrible R joke on twitter that seemed to take off](https://twitter.com/ZKamvar/status/1575563581978210304?s=20&t=aOZbpMH4WdMboiQCx40omQ)

### Date: 2022-09-23

#### Who did you help this week?

I don't think I ended up helping anyone this week 😞

#### Who helped you this week?

 - Toby helped me by talking me down from a depressive episode and considering a different angle for the R Consortium grant
 - Omar and Toby helped me by leaving helpful comments on the Dovetail blog post
 - Karen, Alycia, Kelly, Toby, and Sher! helped me by bringing my request for strategies for community member tasks to their respective meetings
 - Yanina helped me by talking with me about the scope of my R Consortium Grant Proposal

#### What did you achieve?

I was out for a day this week due to mental health issues, so my productivity is not really there. I acheived some of the goals I set out to achieve from last week, but some of them are still just out of reach.

 - [{tinkr} reviewed a pull request to flag attributes in curly braces (useful for passing text to translation APIs)](https://github.com/ropensci/tinkr/pull/76)
 - [{tinkr} merged a pull request that protects square braces from being escaped (yuge deal)](https://github.com/ropensci/tinkr/pull/78)
 - [{sandpaper} merged sandpaper 0.10.0 to create a no-prefix default for lessons](https://github.com/carpentries/sandpaper/pull/333)
 - [{sandpaper} discussed issue of default title for index page WRT LC lessons that do not need setup](https://github.com/carpentries/sandpaper/issues/339)
 - [(docs) added deployment strategy writeup for the workbench](https://carpentries.github.io/workbench/workflow-guide.html#remote-workflow)
 - [Publish Dovetail Number 7](https://carpentries.org/blog/2022/09/dovetail-007/)
 - [R-ecology-lesson (tidyverse-first) made small tweaks to improve the lesson content](https://github.com/carpentries-incubator/R-ecology-lesson/pull/13)
 - [(lesson development training) alerted authors of the lesson to changes in sandpaper](https://github.com/carpentries/lesson-development-training/issues/146)
 - [Begun the proposal for the R Consortium ISC](https://github.com/zkamvar/isc-proposal), with initial [details in twitter thread](https://twitter.com/ZKamvar/status/1573363038669111298?s=20&t=QPYNXqcS4n449La8Je-i6A)
 - Investigated the SSI fellowship
 - Sent out request for help with the Workbench Beta Project
 - Rebuilt and uploaded the beta test repositories to <https://github.com/fishtree-attempt>

#### What did you struggle with?

HOO BOY I struggled a lot with my own brain sabotaging me. As I was talking to my therapist on Wednesday, she said straight up "That sounds like depression." 
It turns out [this depressive episode happened last year as well](Notes-2021.md#date-2021-09-17).
I think I also struggled with trying to write a proposal. The twitter thread above took me a good half hour to write and what I have in that repository is garbage.

#### What would you like to work on next week?

 - Write initial draft of R Consortium grant proposal
 - Get feedback on R Consortium grant proposal
 - Rewrite R consortium grant proposal
 - Submit R consortium grant proposal
 - Come up with project for SSI fellowship
 - Record 6 minute video for SSI fellowship
 - Meeting with Alycia and Kelly about assessment for the beta phase.
 - Cybersecurity meeting
 - Think about the future (R&R day)
 - Investigate creating a Topicbox for Beta Phase updates.
 - Transfer data-lessons/lesson-transtion to the carpentries organisation and work on a new conversion.

#### Where do you need help from Kari?

Not sure. I need help, but I'm not sure where and I don't want to burden anyone else with figuring it out. 

#### What did you learn this week?

Not sure.

#### Any other topics

Next week is going to be really stressful

### Date: 2022-09-16

#### Who did you help this week?

I helped Michael by reminding him to merge the pull requests that [The 
Carpentries Apprentice](https://github.com/carpentries-bot) made to update his
lesson components. I tried to help Janetta by debugging a lesson repository she
created, but it was odd. I helped Toby by typing up participant reactions during
our session at RSEcon22.

#### Who helped you this week?

- Alycia, Karen, Sher!, and Erin helped me out by responding to my request for
  help with the Workbench Beta Phase 🥳
- Maneesha helped me by scheduling our meeting with the Cybersecurity consultant
  for the end of September
- Toby helped me by introducing me to a bunch of people at the RSE conference

#### What did you achieve?

These last two weeks was relatively light in terms of tangible acheivements
because of conference attendance, travel, and a small vacation, but
I will highlight some things that are relevant.

 - Sent out call for help with Workbench Beta Phase Project
 - Attended RSEcon22
 - Exposed more people to The Carpentries
 - Gave away all of my extra Carpentries swag
 - [updated working with the workbench sections of the RSEcon22 workshop](https://github.com/tobyhodges/rse22-workshop-carpentries-workbench/pulls?q=is%3Apr+is%3Aclosed+author%3Azkamvar)
 - Taught 3 hour workshop with Toby that was not without hiccups, but was well-recieved.
 - Had discussions with folks responsible for [Citation File Format](https://citation-file-format.github.io/) about metadata and lesson credit
 - [(documentation) raised issue about homebrew installations](https://github.com/carpentries/sandpaper-docs/issues/104)
 - [{sandpaper} fixed new bugs due to a new version of {cli}](https://github.com/carpentries/sandpaper/pull/337)
 - [{pegboard} fixed new bugs due to a new version of {cli}](https://github.com/carpentries/pegboard/pull/98)
 - [{tinkr} reviewed a new feature to protect attributes in curly braces when sending XML to a translation API](https://github.com/ropensci/tinkr/pull/76)
 - [{sandpaper} proposed `strip_prefix()` function which will remove the numbers from episode names, and thus rely on explicit addition of the episodes to the schedule](https://github.com/carpentries/sandpaper/pull/333#commits-pushed-1698640)

#### What did you struggle with?

I struggled a lot with teaching in person. We realised too late that we could not
provide a collaborative document just in time for the workshop because we were
communicating primarily in meatspace. I think I'm also struggling a bit with
tracking my time because I have a hard time categorising things in different
buckets (which is why I never got in to systematics).

#### What would you like to work on next week?

 - Signalling to the different teams associated with The Workbench what aspects I would like them to bring to their team meetings.
 - Dovetail blog post (once again overdue!) to describe reoganisation and potential new schedule :grimace:.
 - Investigate creating a Topicbox for Beta Phase updates.
 - release sandpaper 0.10.0, which will make episodes without numbered prefixes the default.
 - Transfer data-lessons/lesson-transtion to the carpentries organisation and work on a new conversion.

#### Where do you need help from Kari?

I don't think I need any help in particular, time tracking is weird for me, but I'm learning.

#### What did you learn this week?

The Workbench is nice because it reverses the roles for installation pain to
preview a lesson where it was a pain on MacOS and Windows to now only being a
kind of pain on Linux. That being said, I realise that I should have provided
installation instructions for the specific R packages _before_ the workshop so
that people could be prepared. 

I also learned that a lot of people think that the design of The Workbench makes
sense.

#### Any other topics

I'm definitely not out of the woods in terms of planning, but I have a month to
go before I'm set to deploy the first beta version of the lesson and I think it
will ultimately be fine. I have the team alerted to what I'm doing, I'm going to
update the community about what I'm doing, and initial response to The Workbench
has been good so far. One thing that has happened that I had not planned for is
that Michael has taught the Beta version of his rewrite of the R for Ecologists
lesson, which was written with The Workbench in the first place. I need to work
with him and someone else to figure out how to extract useful information from
workshops like that.

### Date: 2022-09-02

#### Who did you help this week?

I helped Maneesha by putting a note about certificates in the tech channel for when we deploy new badges.
I also helped Erin by fixing and running the script for the alt-text acc-a-thon. 

#### Who helped you this week?

- Toby helped me by talking me off an anxiety cliff about the management of the
  Workbench Beta Phase and helping me understand that the
  `lesson.<program>.org/<lesson>` URLs were an extra, complicated goal for our
  workbench rollout and that the alternative (keeping the `.github.io` urls)
  would be much less disruptive. 
- Kari helped me by pointing out that I am not voluntelling people for their
  help, I am just asking for help and people will give it if they know how much
  time is expected. 
- Kari also helped by being immensely patient with me as she walked through my
  time management processes and said 'this u?'
- Omar gave me a link to the youtube video for the skillup toby and I did.
- Alycia assured me that even though I'm going to sign up for my community
  discussion late, it's not _that much_ of a burden for her to add it to the
  calendar

#### What did you achieve?

This week was a whirlwind! First and foremost, I used the Project Template in 
Asana to create a project board for The Workbench Beta phase, cried a little, 
and then came up with a relatively stable plan that hopefully others can act on.

Here's a breakdown:

 - Created Workbench Beta Project in Asana
 - Created Workbench Roadmap in Asana (not populated)
 - I successfully increased the storage capacity of our build server on AWS (grubmling all the way!)
 - [(carpentries/systems) attempted to fix a bug in our codimd renewal cron job](https://github.com/carpentries/systems/pull/145)
 - [Updated the lc-openrefine styles (3 years out of date)](https://github.com/LibraryCarpentry/lc-open-refine/pull/247)
 - [{sandpaper} added support for custom classes and ids in links and images](https://github.com/carpentries/sandpaper/pull/334)
 - [{sandpaper} opened PR to revamp how episode names are created by default](https://github.com/carpentries/sandpaper/pull/333)
 - [(carpentries/alt-acc-a-thon) fixed and uploaded the script François wrote for the alt-acc-a-thon](https://github.com/carpentries/alt-acc-a-thon) (Thinking about making this public)
 - [workbench documentation: reviewed Toby's contribution to clarify image attributes](https://github.com/carpentries/sandpaper-docs/pull/101)
 - [(carpentries/feeds.carpentries.org) add `EXIT_STATUS` environment variable to track exit status without preventing feeds to be updated](https://github.com/carpentries/feeds.carpentries.org/pull/62)
 - [(cdh.carpentries.org) fix deployment of this page](https://github.com/carpentries/curriculum-development/commits?author=zkamvar&since=2022-08-29&until=2022-09-03)
 - [{pegboard} found an issue with pasted HTML and pandoc markdown that should be flagged](https://github.com/carpentries/pegboard/issues/96)

#### What did you struggle with?

I struggled a lot with project planning and the concept of asking for help is
not burdening people. They are free to reject my request at any time. 

#### What would you like to work on next week?

 - Investigate AWS training opportunities
 - Dovetail blog post! :grimace:
 - Workshop with Toby! :smile: 

#### Where do you need help from Kari?

Nowhere while Im travelling

#### What did you learn this week?

I learned that it is okay to ask people for help. 

#### Any other topics

Nope!

### Date: 2022-08-26

#### Who did you help this week?

I helped Danielle by investigating Topicbox shenanigans. I provided some
guidance around checking images for spoofing to a member of the maintainers
community. I helped give Raniere access to Slack after he lost his password. 
I showed Mateusz where he could find the transformation tool for the workbench.
I helped Toby and the Curriculum team by presenting at the West Pacific time
zone membership council meeting and debugging etherpad when it went down. 

#### Who helped you this week?

Toby helped me by talking with me on Tuesday about The Beta Phase planning. Kari
helped me by pushing me a bit outside of my comfort zone in terms of planning.
I anti-helped Kari by tagging her to review a blog post only a day before it was
supposed to go out. Omar and Toby helped by reviewing said blog post.

#### What did you achieve?

 - [Workbench Documentation: I updated some of the transition guide pages to include descriptions of how the navigation changed](https://carpentries.github.io/workbench/transition-guide.html#navigation)
 - [{varnish} I updated the README to make it more clear for folks who want to fork it](https://github.com/carpentries/varnish/issues/58)
 - [{sandpaper} I fixed a superficial smudge and updated the bioschemas version](https://github.com/carpentries/sandpaper/pull/332)
 - [{sandpaper} I started on functionality to address the user interface to creating episodes and changing their order](https://github.com/carpentries/sandpaper/pull/333)
 - I gave [the 2022-08-25 lab meeting](https://codimd.carpentries.org/Y6SaG9GKTjSp8FbfiITfNA) which was well, received by everyone.
 - I gave the presentation for the Curriculum Team updates for the Member Council on Tuesday
 - I sat on four hiring panels
 - I know I worked on Beta Phase Planning, but it's not in Git, so no linkie.
 - I worked on gathering information for the BSSw fellowship that may or may not be worthwhile.

#### What did you struggle with?

Planning the Beta Phase, I think. Also trying to come up with conferences that
would be good for speaking engagements is hard because I'm still at the point of
I don't know what I don't know. 

#### What would you like to work on next week?

 - Create Workbench Asana Project
 - Investigate AWS training opportunities
 - Finalise strategy for communication and feedback during the Beta Phase of the workbench: review communications document from CT meeting and identify contact people in each community.

#### Where do you need help from Kari?

A suggestion of places where I can best represent The Carpentries.

#### What did you learn this week?

I learned that detecting malware in images is hard 

#### Any other topics

Starting my day hella early and ending it hella early can be nice!


### Date: 2022-08-19

#### Who did you help this week?

I attempted to help Alycia troubleshoot a weird formatting error in the Eventbrite
emails, but I couldn't because eventbrite is the devil. I (perhaps foolishly)
agreed to present on the updates from the Curriculum Team for the second of the
Member council meetings so that Toby doesn't have to get up at 4AM. I addressed
a helpdesk request that turned out to be allowing github access to AMY for a
community member. 

#### Who helped you this week?

 - Kari and Sher helped me by being quick on the draw with the Zoom phone number
   when my internet cut out
 - Kari helped me a lot by giving me examples of large-scale projects and
   reminding me about the communication plan that was due today
 - Sher and Erin helped me out by having good focus during our candidate discussions.


#### What did you achieve?

It doesn't look like I did much this week, but I swear these are all lies. I
just had a lot of meetings, but that _still_ doesn't excuse me becuase everyone
has a lot of meetings. 
 
 - [(actions) updated dependencies](https://github.com/carpentries/actions/commits?author=zkamvar&since=2022-08-15&until=2022-08-20)
 - [(glosario) added a netlify link that got us an Open Source tier subscription](https://github.com/carpentries/glosario/pull/522)
 - [{tinkr} (backend for {pegboard}) released to CRAN](https://github.com/ropensci/tinkr/pull/73)
 - [{pegboard} update for new {tinkr}](https://github.com/carpentries/pegboard/pull/94)
 - [fixed François' name in my talk 😭](https://github.com/zkamvar/rstudio-conf-2022/commit/73c1ddd43ee4a5a610a0db798c243ea19c269c30)
 - [(curriculum development handbook) discovered that the deploy process is broken and needs investigation](https://github.com/carpentries/curriculum-development/issues/75)
 - [(R-Universe) addressed bug due to new {pegboard}](https://github.com/r-universe-org/help/issues/190)
 - Interviewed five candidates for the DoT position
 - addressed the tasks in the [Workbench Beta Phase Planning](https://app.asana.com/0/1166476597848794/1202647304529920)


#### What did you struggle with?

I think I struggled a bit with submitting {tinkr} to CRAN because they kept
coming back with false-positive tests for what was going on and it was a 
frustrating cycle of submitting, getting rejected for a thing that did not exist
and getting asked to resubmit, and then getting dinged on a new thing. 

I also struggled a bit with focusing the plan for the Beta Phase communication.
It still seems disconnected in a way. 

#### What would you like to work on next week?

 - Investigate AWS training opportunities
 - Come up with project plans to use for applying to [the BSSw Fellowship Program](https://bssw.io/blog_posts/applications-open-for-the-2023-bssw-fellowship-program)
 - Finalise strategy for communication and feedback during the Beta Phase of the workbench: review communications document from CT meeting and identify contact people in each community. 
 - Prepare for lab meeting (building workbench lessons locally or on RStudio cloud)

#### Where do you need help from Kari?

 - Nowhere specific.

#### What did you learn this week?

I learned that I really really really really really should have created an asana
project for The Workbench at the beginning of the year when I was thinking about
the Beta Phase.

#### Any other topics

One of the things that is still eating at me is the concept of trying to set up
feedback mechanisms for The Workbench for instructors and potentially learners.
At the moment, I have the idea that I would get feedback via mock teaching demos,
but there is a big question of how exactly to organise something like that and 
how the community would receive/participate in these. I'm also realising that
this quarter was supposed to be the quarter in which we officially started the 
Beta Phase of The Workbench, but it fell through the cracks due to _several_
factors. One thing that is the same between now and three months ago is that we
now have a call for Community Discussions and I know that this is a big way to
reach out to the instructor community and they can be successful if advertised
early and often, but I currently do not have a plan for these for The Beta Phase
yet again and I do not want these community discussions to turn out like they
did at the beginning of this quarter with no clear agenda and low turnout. It 
might be better since we aren't working on CarpentryCon anymore, but I'm not
sure. When it comes to communicating with the community, it definitely feels
like this is one of my weak points (and not for a lack of trying). 

### Date: 2022-08-12

#### Who did you help this week?

I helped Alycia find the right login for eventbrite and forwarded an email to
Erin so that she could invite a person from the translation panel to participate
in community interviews. I stepped in to moderate a session for Erin when she 
was feeling under the weather. 

#### Who helped you this week?

 - Alycia helped me by being so on top of things and giving me heads up about
   sessions I was participating in (e.g. translation session). She also
   reminded me that we can choose which recording we want to upload for Toby
   and my session (because mine was hot garbage). 
 - Toby helped me by running his solo intro to the workbench smoothly and
   reporting back.
 - Maneesha helped me by coworking on an AWS mystery.

#### What did you achieve?

If I am drained this week, I have no clue how the rest of y'all are still standing.

 - I gave three CarpentryCon Skillup sessions, sat on one panel, and facilitated one small session
 - [{sandpaper} I released a version that includes anchor links for the headings](https://github.com/carpentries/sandpaper/pull/325)
 - [{varnish} added a border around the mobile navbar menu for better visibility](https://github.com/carpentries/varnish/pull/57)
 - [{varnish} fixed sidebar behavior and label](https://github.com/carpentries/varnish/pull/57)
 - [{varnish} fixed heading sizes and callout underlines](https://github.com/carpentries/varnish/pull/55)
 - [{tinkr} (backend for {pegboard}) prepared a release to CRAN](https://github.com/ropensci/tinkr/pull/73)
 - [found a incompatibility bug in quarto](https://github.com/quarto-dev/quarto-cli/issues/1854)
 - [add my RStudio talk to my personal site](https://github.com/zkamvar/zkamvar/commits?author=zkamvar&since=2022-08-08&until=2022-08-13)
 - Updated some documentation in {sandaper} [for configuration variables](https://carpentries.github.io/sandpaper/reference/set_config.html#details)


#### What did you struggle with?

My previous entry really says it: a lot of things that I can not really name
right now. It's just a morass of feels that are really difficult to deal with. 


#### What would you like to work on next week?

* First interviews for DoT position.
* Plan for Workbench Beta Phase

#### Where do you need help from Kari?

* I need help thinking about what I can prepare for the upcoming CT discussion on
  "Communciations Planning around long term projects" that I submitted sometime
  before I went on conference/vacation

#### What did you learn this week?

I learned that Netlify has an open-source plan that's much easier to apply for
than begging for credits from AWS. I also learned that people who know about the
carpentries are always really impressed by the work our volunteers do and people
who haven't heard of the carpentries are impressed by the model and dedication:
https://twitter.com/philosohacker/status/1556388481504624640?s=20&t=xQonVQp2Zlczmfof8WgoWQ

#### Any other topics

AWS people were at the RStudio conference, but I did not talk to them `-_-` I
am always weirded out by going up to someone and asking for support in the form
of free credits (even though it's A M A Z O N.... i mean). 

I also appreciate the efforts to de-stress the team. It's been a tough month for
sure. 

### Date: 2022-07-22

#### Who did you help this week?

I helped Erin by removing the metadata from the hiring committee documents, 
because they were not anonymized (this is a common thing and I think the 
solution is for anonymizers to make sure to export the anonymized version as a
new PDF). I helped Janetta at the beginning of the week by addressing a couple
of glosario pulls. 

#### Who helped you this week?

The whole team really helped me by validating that the presentation I had
created accurately represented us. Karen helped my by providing images; Toby
scheduled a session with me to discuss my Job Description in terms of the
Curriculum Team. Talisha reminded me that I had not yet submitted my responses
for the community calls I lead (I blame google). Kari got me to actually look
at my Job Plan in two months :grimace:. Erin and Toby talked me down from my
mild panic at realising that I'm having a difficult time reconciling what I am
doing and what I'm _supposed_ to be doing (in terms of Curriculum Team).

#### What did you achieve?

This week was mostly spent writing my slides/practising my talk.

 - [I finished my RStudio conference slides](https://zkamvar.github.io/rstudio-conf-2022/)
 - [I wrote dovetail issue number 5 where I announced the beta phase on hold](https://github.com/carpentries/carpentries.org/pull/1450)
 - [I added context to a question Sarah Brown had for François about lesson release](https://github.com/carpentries/instructor-training/pull/1412#discussion_r923507403)
 - [I prepared an intro to workbench slide deck for the session Toby and I are leading](https://docs.google.com/presentation/d/1L4CSpp-T2q-qXq_N4oMbRx9bklMgXL5bR_jmxTWy4L8/edit?usp=sharing)


#### What did you struggle with?

A lot of things that I can not really name right now. It's just a morass of feels
that are really difficult to deal with. 

#### What would you like to work on next week?

* RStudio conference!
* DoT Application reviews (all 20 of them!)

#### Where do you need help from Kari?

* Not at the moment.

#### What did you learn this week?

My slides have images as the background, but the catch is that [they are not
detected by screen readers](https://twitter.com/ZKamvar/status/1549449295790686208?s=20&t=9VaeQFTcytKd541lURouOQ),
I found out how to add test that is visually hidden, but I found out that it is
better to [include an empty `<img>` tag with alt text so that screen readers 
recognise it as an image](https://twitter.com/shipman/status/1549499936013778952?s=20&t=9VaeQFTcytKd541lURouOQ).

#### Any other topics

Stress is still high, but I have a lot more confidence in my talk now :)

### Date: 2022-07-15

#### Who did you help this week?

Kind of a cop-out, but I helped Toby by forcing him to cancel the Instructor
Notes drive, which gave him time to work on other things. I also cancelled my
final 1:1 with François to allow him to rest at 6PM on his last day. 

#### Who helped you this week?

Where do I start? Omar helped me by providing the tri-hex for the carpentries
workbench with a transparent background so that I could use it in my slides.
Erin attended my community discussion on Monday, Karen helped me by talking 
with me Wednesday morning and helping me determine that I needed to push back
the beta testing of the workbench (subsequently, this also helped Karen make up her mind on a task as well). François, Toby, and Sarah Stevens provided
tesimonials for me to use in the workbench presentation. Toby assured me that
postponing the beta phase was the right choice. Kari shared her slides that
talk about our core values so that I could adapt them to my talk. Kari helped
me recognise that I needed to be more open about my questions when I
encounter them instead of waiting until I'm overwhelmed. 

#### What did you achieve?

 - [I put the Workbench Beta phase on hold until mid-august](https://github.com/carpentries/workbench/discussions/22)
 - [I made a lot of progress on my RStudio conference slides](https://zkamvar.github.io/rstudio-conf-2022/)
 - [{sandpaper} version 0.9.0 is released with AWS deployment and an improvement to `set_dropdown()`](https://github.com/carpentries/sandpaper/releases/tag/0.9.0)
 - [(lesson-transition) found a bug with my R-ecology-lesson script](https://github.com/data-lessons/lesson-transition/issues/8)
 - [{varnish} fixed lists in solutions that did not have style](https://github.com/carpentries/varnish/pull/52)
 - Hosted a community discussion to 1 (one) person in the Oceania TZ. 


#### What did you struggle with?

* I struggled a lot with juggling the different priorities that I had. The
  beta phase was not as ready as it needed to be and that's partially because
  I didn't set up a good communication plan. 

#### What would you like to work on next week?

* Get prepared for RStudio conference
* Reassess Workbench Beta Phase plan
* Coordinate with Sher! about instructor communication, testing, and RStudio 
  conf and regular meetings
* prepare for sessions I'm running at CarpentryCon (slides for Toby, outline 
  for Sarah)
* Sleep

#### Where do you need help from Kari?

* The strength to ask for things that I need (this is often the hardest 
  section for me to write).

#### What did you learn this week?

* I learned that it's okay to push things back if they are not ready.
* I also learned that we might be able to get around the wonky underlines 
  that our callout box titles have in the workbench (if the titles wrap,
  then the underline doesn't follow the text exactly because it is offset
  vertically): <https://css-tricks.com/styling-underlines-web/>

#### Any other topics

The name of the game here is survival until mid-September. It's gonna be
busy as all h\*ck, but I don't feel like anyone is pushing me to do things
that I do not want to or can not do. People liked my talk at the practice
session, so I just need to make sure I polish everything before I head out
for my red-eye next week `ㅠ_ㅠ`. I do feel stress right now and it feels
almost the same amount as the stress I've felt during my previous position,
but the key difference here is that I know I can effectively manage this 
stress because I know I have the support from everyone on the team and the
support from the community in ways that manifest themselves as genuine
kindness and concern.

### Date: 2022-07-08

#### Who did you help this week?

I helped Karen by taking notes at the instructor training meetings this week
(which were really informative!). I helped address some issues that were
blocking glosario PRs. I helped Erin by updating some language in the DoT post.
I also took the time to help explain why the output an incubator author was 
seeing was actually expected: https://github.com/carpentries/sandpaper/issues/317

#### Who helped you this week?

François helped me by writing and rewriting copious amounts of documentation for
our infrastructure in a small window of time. He was also super calm and
collected every time I had a panicky question about AWS or asking for logins and
permissions to things. Kari helped me by asking tough but important questions
at our meeting. Kari and François attened my first session for the listening
session. Erin, Alycia, Karen, Kari, and Omar gave me support when I was
momentarily out of my mind after the session. Jannetta Steyn made a joke on
slack that I really appreciated.

#### What did you achieve?

I was wondering why I was tired this week. It turns out I did quite a bit,
covering 117 commits:

 - [(actions) check-valid-pr now has an invalidation parameter and updates messaging](https://github.com/carpentries/actions/pull/50)
 - [{sandpaper}/added enhanced pull request validation that would give better status messages and check if a PR is trying to import a commit after conversion to the workbench](https://github.com/carpentries/sandpaper/pull/316)
 - [{sandpaper} fixed logic for the optional `fail_on_error` parameter](https://github.com/carpentries/sandpaper/pull/315)
 - [{sandpaper} added an AWS deployment workflow](https://github.com/carpentries/sandpaper/pull/318)
 - [(blog) added dovetail number 4](https://github.com/carpentries/carpentries.org/pull/1433)
 - [added invalid-hashes.json to our files subdomain](https://github.com/carpentries/reactables/pull/2)
 - Swapped François' tokens for my tokens
 - Updated the tokens for @carpentries-bot
 - tested out creating an AWS S3 bucket to host lesson websites and in doing so, I 
   + updated the [AWS S3 systems wiki entry](https://github.com/carpentries/systems/wiki/AWS-S3)
   + updated the [CloudFront Setup wiki entry](https://github.com/carpentries/systems/wiki/AWS-CloudFront#Set-up)
   + updated the [machine user systems wiki entry](https://github.com/carpentries/systems/wiki/machine-user)
 - tested out https://lessons.datacarpentry.org/R-ecology-lesson
 - Ran my community discussion for the workbench


#### What did you struggle with?

 - AWS :fire: :fire: :fire:
 - Not being prepared for community discussions
 - feeling guilty for not preparing my talk that's due next week :grimace:

#### What would you like to work on next week?

 - Prepare lesson transition script to do the conversion _with_ force-pushing
   on the test repository to demonstrate what a pull request from an invalid
   fork looks like
 - release lessons.datacarpentry.org/R-ecology-lesson as workbench pre-beta,
   which means giving access to the lesson maintainers.
 - finish my talk :weary:

#### Where do you need help from Karnçi?

 - A good solid hook for introducing The Carpentries
 - Get testimonials from folks about the workbench that I can use at the end
   of my talk (I'm hoping Toby will come trough on this).
 - A resource of visuals that I can use in my talk
 - Do you know if it's possible to download google slides as a PDF? I don't know
   if I will have online access. 

#### What did you learn this week?

- I learned that it is possible for us to generate and upload AWS secrets from
  the command line, but it will take a few hours of work to formalise it. 
  The benefit of this is that we would be able to make sure we can easily
  respond to security breaches by rotating tokens. 

#### Any other topics

I am low-key worried about my talk https://github.com/zkamvar/rstudio-conf-2022

It's still in notes form and slidecraft is HARD. 

### Date: 2022-07-01

NB: I wrote this on 2022-07-04 as I ran out of time on Friday.

#### Who did you help this week?

I helped Alycia with some technical aspects of the CarpentryCon website.

#### Who helped you this week?

François helped me by explaining some of his secrets WRT to the deployment on 
AWS buckets and the process for lesson release. Kari helped me by clarifying her
role as my interim supervisor.

#### What did you achieve?



 - [(lesson-transition) I was able to get the R-ecology-lesson back up and running](https://github.com/data-lessons/lesson-transition/commits?author=zkamvar&since=2022-06-27&until=2022-07-02)
 - [(actions) I added a check in the pull request validator that would help protect migrated lessons from existing lesson forks](https://github.com/carpentries/actions/pull/50)
 - I tested deployment of a lesson website to the `https://lessons.datacarpentry.org/` bucket using the scheme that François came up with.
 - [{sandpaper} I added a config option `fail_on_error` that would fail if an R Markdown document produced an unexpected error](https://github.com/carpentries/sandpaper/pull/310)
 - [workshop template: I reviewed the Covid Protocol addition](https://github.com/carpentries/workshop-template/pull/764#pullrequestreview-1020629849)
 - I tested out the workbench tranisiton process
    - I made a [clone of my thesis R package](https://github.com/zkamvar/laughing-winner)
    - I forked it to my alt account, @ravmakz
    - I ran `git-filter-repo` to remove two configuration files and force pushed
    - I created [a pull request from the fork](https://github.com/zkamvar/laughing-winner/pull/4) and [from the local repo](https://github.com/zkamvar/laughing-winner/pull/5)
      to test the PR validation.
    - I force-pushed the original main branch back to the lesson and [saw the 
      pull requests reverse statuses (check the history), confirming that the
      process _can be_ reversible from the 
      snapshot](https://github.com/zkamvar/laughing-winner/pull/5#issuecomment-1172792190)
  - I estimated the fudget for travel to the RSE conference in September
  - I learned how to provision new sites on AWS and to add one user per folder
  - I learned how the lesson release process works

#### What did you struggle with?

I don't recall struggling that much this week actually

#### What would you like to work on next week?

 - Register RSE conference and purchase flight/accommodation
 - look into freezing pull requests on a repository via GitHub branch protection
 - Modify transition to first push full repo and fork to Zhian’s account (to 
   demonstrate to maintainers what an invalid/outdated pull request looks like
   and how to handle it)
 - Regenerate access tokens via bot account
 - Create `https://files.carpentries.org/invalid-hashes.json` to hold known 
   invalid commit sha hashes after the transition to the workbench. 
   - Maybe mix into https://github.com/carpentries/reactables/ and make public

#### Where do you need help from Krançoi?

Nowhere at the moment!

#### What did you learn this week?

I learned that the `pull_request_target` action trigger is actually useful
because it can not be modified by a pull request and will always run on a pull
request, regardless of who triggers it. This is useful for our Pull Request
Validator action, which will indicate if a pull request is being spoofed or if
it has a combination of modified workflows and content (in which case, it should
definitely not be merged). 

Having the `pull_request_target` workflow means that we can give a quick
valiation to the lesson maintainers/developers about whether they should attempt
to run the lesson or if the workflow may be suspicious.

#### Any other topics

Because I was able to test the situation in which I would be transitioning the
lessons, I am now more confident in my approach. 

### Date: 2022-06-24

#### Who did you help this week?

I helped François review the Bytes.co site and I looked into the budget for
travel to the RSE conference in September to support Toby. I addressed an issue
on the carpentries website WRT external resource permissions. 

#### Who helped you this week?

Toby added a fix for the sandpaper templating process and fixed a test.

#### What did you achieve?

 - [I created a repository for my notes for RStudio conf](https://github.com/zkamvar/rstudio-conf-2022)
 - [{varnish} fixed the navigation in mobile browsers](https://github.com/carpentries/varnish/pull/50)
 - [{sandpaper} fixed navigation in mobile browsers and downlit update](https://github.com/carpentries/sandpaper/pull/309)
 - [Published Dovetail Number 3 establishing the order of lessons to enter beta](https://github.com/carpentries/carpentries.org/pull/1426)
 - Worked on RStudio talk

#### What did you struggle with?

* I struggled a lot with coming up with an appropriate scheudle and trying to
  figure out the best way to transition lessons. I also struggled a lot in
  general with the state of the world.

#### What would you like to work on next week?

* get narrative for my RStudio talk finished
* submit budget for RSE Conference in September
* learn François' secrets
* add option to allow errors to stop a build in the workbench

#### Where do you need help from François?

* I need to know where we can archive repositories before I enter them into the
  beta phase. 

#### What did you learn this week?

* I learned that piecemeal migration of issues is not simple because there are
  things in an issue yaml object after migration that are not part of the issues
  schema (which makes sense because you don't want people mocking issues).

#### Any other topics

* I think we are all going through some really stressful times and I have to
  remind myself that I'm doing the best I can.

### Date: 2022-06-10

Note: this was written on 2022-06-20 and contains information from 06-13

#### Who did you help this week?

I helped Sarah Stevens draft text for her CarpentryCon proposal submission.

#### Who helped you this week?

Hooboy, Kari helped me by checking in on me. Erin helped me by talking with me
before I took sick time this week. Joel and David helped me by understanding
when I had to cancel our meeting.

#### What did you achieve?

I had a bit of a limited week due to my approaching  burnout, but I was able to
get the following completed:

 - [created a list of lessons in workbench Beta Testing](https://github.com/carpentries/workbench/discussions/11)
 - [Created a post about keeping up to date with The Workbench](https://github.com/carpentries/workbench/discussions/12)
 - [{varnish} renamed CHAPTERS to EPISODES](https://github.com/carpentries/varnish/pull/45)
 - [{varnish} Disabled search](https://github.com/carpentries/varnish/issues/42)
 - [{varnish} added persistant state for menu collapse](https://github.com/carpentries/varnish/issues/43)
 - [{sandpaper} update `create_episodes()` to create a slug from the title](https://github.com/carpentries/sandpaper/pull/295)
 - [{sandpaper} add new functions to support markdown-first lessons](https://github.com/carpentries/sandpaper/pull/297)
 - [(lesson-tranistion) did a lot of things to try to make it work on CI](https://github.com/data-lessons/lesson-transition/commits?author=zkamvar&since=2022-06-06&until=2022-06-11)
 - [fixed an error in pkgdown](https://github.com/r-lib/pkgdown/pull/2121)
 - [published dovetail blog post](https://github.com/carpentries/carpentries.org/pull/1418)
 - I helped lead a session of maintainer onboarding and atteneded a DEI call.
 - I attended a call for my RStudio conference talk.

#### What did you struggle with?

I struggled a lot with burnout and also learning about [redacted]. It's a big
change and while I know there are systems in place to make sure everything
keeps running, it's a difficult situation after two and a half years. Luckily I
was able to spot the burnout early enough that it did not begin to affect my
health too much, but it's something that I do need to be careful of. 

I also struggled with figuring out the appropriate time to schedule the testing
and figuring out how to work around the blockers. One of my faults is that I do
not like not knowing the details of a plan that I will be involved in. In this
case, not knowing the details of how the beta lessons would be deployed to AWS
or how the lesson release process works sent me into a negative thought spiral
where I was unable to concentrate on anything but worrying about how I would 
burden my supervisor by asking him to perform these tasks. This is a fault of
mine that I have not effectively communicated or managed and it's really tearing
me a new one.

#### What would you like to work on next week?

Note: this will be for this current week

- Come up with a rough draft of my RStudio::conf talk, centering around the
  carpentries core values
- Come up with schedule for beta testing 
- Add some content to the Moore Grant final report

#### Where do you need help from François?

- sobs

#### What did you learn this week?

I learned that it's okay and necessary to take a step back, even if everything
seems urgent, and disconnect from work. I was getting to the point where I was
not sleeping well and I knew that I needed to disconnect and descramble my brain.

#### Any other topics

François, I want you to know that you are the best supervisor that I've ever
had. You are always the best defence against my self-deprecation and you have
never been less than kind and professional in our work together. 

### Date: 2022-06-03

#### Who did you help this week?

I helped Alycia with reviewing content for the followup blog post on 
internationalisation and I shared the styles/workbench icons with Toby. I also
helped confirm that we could close an issue in our strategic plan repository.

#### Who helped you this week?

Erin helped me by talking through the challenges of doing the maintainer
onboarding with the workbench still in beta. She reminded me that I can submit
a skillup session for The Carpentries Workbench. Toby helped me out by giving 
me support during difficult times. Talisha helped me understand what I need to
do to get stickers ordered for the RStudio conference and for the voulenteers.

#### What did you achieve?

This week was a bit of a slow week because I had taken Wednesday off and reading
and reflection day was spent fighting continuous integration.

 - [(lesson-transiton) I attempted to make this work purely on github actions, but the R resources are killing me](https://github.com/data-lessons/lesson-transition/commits?author=zkamvar&since=2022-05-30&until=2022-06-04)
 - [{varnish} I added a lesson status tag for lessons in pre-alpha to beta](https://github.com/carpentries/varnish/pull/39)
 - [{varnish} add issue to address link validation for a common error with space between braces](https://github.com/carpentries/pegboard/issues/90)
 - [(r-universe) attempt to fix a bug in the r-universe deployment chain](https://github.com/r-universe-org/sync/pull/3)
 - [(workbench documentation) added descritpion for long alt text and decorative images](https://github.com/carpentries/sandpaper-docs/commits?author=zkamvar&since=2022-05-30&until=2022-06-04)
 - [(actions) setup sandpaper even if config.yaml doesn't exist](https://github.com/carpentries/actions/commit/0494391e4cd0059c0a5b9a4c780625e650aa8bc7)
 - [(Lesson Devel Training) Reviewed draft of operations episode](https://github.com/carpentries/lesson-development-training/pull/47)
 - [(maintainer onboarding) I started a pull request to update chapter 4](https://github.com/carpentries/maintainer-onboarding/pull/63)
 - I reviewed the new website layout

#### What did you struggle with?

* I struggled a lot with continuous integration
* I also struggled a lot with prioritizing things in the light of needing to
  get the transition script ready and prepping the beta phase volunteers.

#### What would you like to work on next week?

Next week is a long week with a potential for 16 hours of that week in meetings.

* write and publish the Dovetail
* Update my job plan for May and June
* Contact beta phase volunteers about when we can expect to start
* Schedule a vacation at the end of June

#### Where do you need help from François?

 - provide a realistic timeline for when the new URLs will be available. It's
   okay if we have to delay.

#### What did you learn this week?

* I don't recall finding out anything terribly new.

#### Any other topics

I am realising that I have taken a single day off in the last two months. This
on top of everythign that's been going on... I can say that I think I'm starting
to burn out. The problem is that I have a lot of time-sensitive things that I
need to work on and a lot of things that are pulling me in different directions.
Because of this, it seems like there is never going to be a good time for me to
take a rest in the next few months, especially if we get the beta phase going.

I noticed that the last time I had a vacation was the end of March and the last
time that I had commits straight through for two months was August to October
2021 in which I was hella tired and rundown by the end of it. 

### Date: 2022-05-27

(note: written on 2022-05-30)

#### Who did you help this week?

 - I helped Saba track down an error in a lesson build (it turned out to be a 
   DNS issue with CRAN and RStudio)
 - I helped Erin by posting the final call for maintainer applications to twitter
 - I found a real-world example of using variables in the website.

#### Who helped you this week?

 - Alycia helped me by running and organising the translation community call this week
 - Alycia helped me by running and organising the data sovereignty meeting without me this week
 - The Core Team helped me by giving me honest feedback about what they knew and didn't know about The Workbench

#### What did you achieve?
 
 - Demonstrated The Workbench to participants at the Research Software Camp
 - Lead the Lab Meeting for the week
 - I got 16 responses for the Beta Phase of the Workbench with 9 followups (5 incubator maintainers, 2 maintainers, 2 instructors)
 - [I wrote and published the first dovetail blogpost](https://github.com/carpentries/carpentries.org/pull/1416)
 - [{sandpaper} updated pr-receive workflow to emit {pegboard} checks when processing](https://github.com/carpentries/sandpaper/pull/291)
 - [{sandpaper} removed outdated content in update workflows](https://github.com/carpentries/sandpaper/pull/292)
 - [(actions) use job summaries for validation workflows](https://github.com/carpentries/actions/pull/45)
 - [{pegboard} added summary methods and message muffler for Lesson and Episode objects](https://github.com/carpentries/pegboard/pull/89)
 - [carpentries.org added .vendor to .gitignore](https://github.com/carpentries/carpentries.org/pull/1417)
 - [reviewed a PR from Sarah Stevens for the workbench documentation](https://github.com/carpentries/sandpaper-docs/pull/86)

#### What did you struggle with?

 - This was a very diffuclt week emotionally. I took a half day on Thursday to
   recover mentally.
 - I struggled with trying to define and set my own boundaries with what is
   possible for me to support in terms of the beta phase. 

#### What would you like to work on next week?

 - draft testing plan timeline for the beta phase participants
 - modify lesson transition tool to have specific pathways
 - write up deployment strategy for the beta phase
 - add general 'asis' node fixer for {tinkr}
 - release {tinkr} to CRAN
 - review new Carpentries Website Layout

#### Where do you need help from François?

 - Implement one-to-one user/repo deployment of beta phase lessons on the AWS
   side.

#### What did you learn this week?

 - I learned that there is no hard and fast rule for how long alt text should be
   <https://css-tricks.com/just-how-long-should-alt-text-be/>

#### Any other topics

This summer is definitely going to be pretty heavy.

### Date: 2022-05-20

#### Who did you help this week?

 - I helped validate Alycia's thoughts about the i18n call next week
 - I addressed some slack helpdesk issues

#### Who helped you this week?

 - Toby and Erin helped me understand how the maintainer onboarding call and the
   workbench beta call fit in and complement one another
 - Sher! and Erin helped me understand the bounds of what we can and cannot
   accomplish with the workbench beta phase in terms of COW. 

#### What did you achieve?

 - [{downlit} I fixed a small bug in downlit](https://github.com/r-lib/downlit/pull/138)
 - [{sandpaper} I fixed a small bug with rendering the R-raster-vector-geospatial lesson](https://github.com/carpentries/sandpaper/pull/289)
 - [{sandpaper} fixed a small bug where ampersands in titles would cause the AIO page to not be built](https://github.com/carpentries/sandpaper/pull/287)
 - [{varnish} testing out alert banner for beta phase](https://github.com/carpentries/varnish/pull/38)
 - [{pegboard} added a kludge for a situation where captions contain URLs and are parsed by markdown](https://github.com/carpentries/pegboard/pull/87)
 - [{tinkr} added workflows](https://github.com/ropensci/tinkr/pull/70)
 - [{tinkr} started drafting a namespaceless tinkr (need refactor for pegboard, tho)](https://github.com/ropensci/tinkr/pull/69)
 - [trainer-training: updated styles](https://github.com/carpentries/trainer-training/pull/49)
 - [added backgrounds to the brand identity page on our docs](https://github.com/carpentries/docs.carpentries.org/pull/842)

#### What did you struggle with?

I struggled with a lot. Part of my struggle was trying to come to terms that I
really can not take on much more work. Another part was trying to refactor
{pegboard} to not use namespaces... it's going to take a bit more time. This is 
all on top of trying to figure out what _exactly_ to do with the beta phase.

#### What would you like to work on next week?

 - I want to create a test lesson with issues and pull requests that I can use to demonstrate the transition
 - Add workbench beta alert to the lessons in beta
 - Send communication to the respondents of the beta phase

#### Where do you need help from François?

 - Nowhere right now

#### What did you learn this week?

 - bootstrap has a dismissable alert that works pretty well with our site... but the close button gets obscured because of our CSS `-_-`

#### Any other topics

None. I'm tired.

### Date: 2022-05-13

#### Who did you help this week?

Replace this text with a one/two sentence description of who you helped this week and how.

#### Who helped you this week?

Replace this text with a one/two sentence description of who helped you this week and how.

#### What did you achieve?

 - [(lesson-development-training) addressed several questions from Toby](https://github.com/carpentries/lesson-development-training/pull/41)
 - [(sandpaper-docs) added a component guide](https://github.com/carpentries/lesson-development-training/pull/41#discussion_r868190338)
 - [{sandpaper} diagnosed an issue with the package cache that was brought up by LearnToDiscover](https://github.com/carpentries/sandpaper/issues/283)
 - [{pegboard} updated `fix_links()` to process headings](https://github.com/carpentries/pegboard/pull/86)
 - [{varnish} fixed a visual bug where the navbar dropdown would be covered by the sidebar](https://github.com/carpentries/varnish/pull/36)
 - [(instructor-training) fixed non-compliant mailto links](https://github.com/carpentries/instructor-training/pull/1368)
 - [(maintainer-onboarding) reviewed Erin's changes](https://github.com/carpentries/maintainer-onboarding/pull/62)
 - [(incubator/metagenomics) diagnosed an issue where math support was missing](https://github.com/carpentries-incubator/metagenomics/issues/31#issuecomment-1125509310)
 - [(blog post) addressed comments from Annajiat](https://github.com/carpentries/carpentries.org/commits?author=zkamvar&since=2022-05-09&until=2022-05-14)
 - [(workbench documentation) updated folder structure image to match content](https://github.com/carpentries/workbench/commit/7e09ebce0ba59f52297da4005c1e0b5b68e98244)
 - [(workbench) had the beginning of a discussion about i18n during the beta phase and the challenges therein](https://github.com/carpentries/workbench/discussions/6)
 - I Communicated about the Beta Phase to the Alpha testers and the various communities
 - I reran the lesson transition script

#### What did you struggle with?

 - I struggled a lot with trying to figure out how to respond about i18n during
   the beta phase. It was difficult for me to come up with the right way to
   emphasise that it is a priority, but I need more time and discussion in
   order to properly implement it. 

#### What would you like to work on next week?

 - I want to create a test lesson with issues and pull requests that I can use to demonstrate the transition
 - I want to bump my call for maintainers because right now I have a total of seven :grimace:

#### Where do you need help from François?

I need to understand how the new URLs will work. The matomo integration that we
are using for the workbench is assuming that we have `lessons.carpentries.org`,
but when we discussed the beta phase, we had the urls going to 
`lessons.<program>.org`. It's not a big deal to change the matomo settings, but 
I think we really need to hash out what our expectations for the final URLs are
with versioning and i18n included:
<https://github.com/carpentries/sandpaper/issues/216> because at the moment, I
feel like we don't have a solid grasp of what we want to do and are making
quick changes without taking into account the full scope of work.

#### What did you learn this week?

- I learned that I still freeze up when tasked with communicating about large
  and complex topics.

#### Any other topics

I realise that my timing with the beta phase is... well... bad. The reason I
know it's bad is because Erin is recruiting for Maintainer onboarding for June.
So, we are going to have potentially 25-50 maintainers onboarded who are
learning the styles version of the lesson and then have to re-train to switch to
the workbench if the previous maintainer elect to switch to the workbench. :weary:

### Date: 2022-05-06

#### Who did you help this week?

 - I contributed to a discussion about translations for The Workbench.
 - I clarified how folks should use equations inside the incubator template

#### Who helped you this week?

 - Karen and François gave me feedback on the blog post
 - Erin clarified the data she entered into AMY (so that I can use that as the
   primary source for removing access for maintainers who have stepped down)
 - Erin, François, and Toby helped me with a discussion about terminology in
   the workbench.
 - Karen and Maneesha reminded me about how to give a task to multiple people
   and we jointly discovered that Asana is subtly fucking with us.

#### What did you achieve?

 - [(workbench) I authored a transition guide between the workbench and styles](https://carpentries.github.io/workbench/transition-guide.html)
 - [I finalized and published the blog post about the beta phase](https://carpentries.org/blog/2022/05/workbench-beta/)
 - [{varnish} added lab and incubator logos](https://github.com/carpentries/varnish/pull/30)
 - [{varnish} add blockquote styling](https://github.com/carpentries/varnish/pull/31)
 - [(actions) added quickfix and backup for the R-universe API](https://github.com/carpentries/actions/pull/42)
 - [(actions) more reliably enforce RSPM availability on runners](https://github.com/carpentries/actions/pull/43)
 - [{sandpaper} updated workflows to no longer install R from external sources; use v2 of the r-lib actions; set GITHUB_TOKEN permissions](https://github.com/carpentries/sandpaper/pull/279)
 - [(workbench forum) answered a question about tabsets in the workbench](https://github.com/carpentries/workbench/discussions/5#discussioncomment-2701675)
 - I presented the beta phase to the trainer community
 - I re-ran the lesson transition script and fixed some assumptions (e.g. changing guide.md -> instructor-notes.md)

#### What did you struggle with?

 - I didn't struggle that much this week. I took time off when I needed to take
   time off. I think a lot of struggle was again prioritisation, but it's
   minor.

#### What would you like to work on next week?

 - Communicate about the Beta Phase to the Alpha testers and the various communities
 - Update the lesson transition script and add some more lessons
 - Create an example of a repository transition 

#### Where do you need help from François?

* nowhere at the moment

#### What did you learn this week?

 - Mermaid diagrams ARE possible in our infrastructure and they work similar to 
   how mathjax is processed! https://css-tricks.com/making-mermaid-diagrams-in-markdown/

#### Any other topics

Emergency vet bills can escalate rather quickly!

### Date: 2022-04-29

#### Who did you help this week?

I helped Erin by fleshing out the Curriculum section in the annual report blog post when she was feeling overwhelmed.
I additionally reviewed content for Sarah Stevens. 
I made a PR for Matt's lesson that properly tagged it as a data carpentry lesson.

#### Who helped you this week?

François, Erin, Michael, and Karen helped me by giving me feedback on my beta blog post.
Omar gave me appropriate context for scheduling a blog post. 

#### What did you achieve?

 - [(workbench beta) I documented how to create a friction log](https://github.com/carpentries/workbench/discussions/2)
 - [(workbench blog) I drafted the workbench beta blog post](https://github.com/carpentries/carpentries.org/pull/1375)
 - [(workbench discussion) I created a discussion forum and comparison document (incomplete) for the workbench](https://github.com/carpentries/workbench)
 - [(workbench documentation) I addressed missing documentation for code blocks](https://github.com/carpentries/sandpaper-docs/issues/80)
 - [(docs.carpentries.org) I updated the markdown parser](https://github.com/carpentries/docs.carpentries.org/pull/838)

#### What did you struggle with?

 - I struggled a bit with prioritisation and trying to find balance between getting things done and getting things perfect.

#### What would you like to work on next week?

 - Update the lesson transition script and add some more lessons

#### Where do you need help from François?

* nowhere at the moment

#### What did you learn this week?

* The neovim that comes from debian has bug that can trap you in insert mode after pasting certain characters: https://github.com/neovim/neovim/issues/11699

#### Any other topics

Nope! I'm done for the week!

### Date: 2022-04-22

#### Who did you help this week?

 - I uploaded my excalidraw library for Alycia
 - I clarified the Beta Phase of the Workbench Transistion to the maintainers

#### Who helped you this week?

 - Dan asked a really good question about how to re-train maintainers
 - Omar addressed my question about putting our logo in a public library 

#### What did you achieve?

 - []()
 - I spoke with the Instructor Development Committee about beta phase testing
 - [I organised the phases of the transition plan](https://docs.google.com/document/d/1EMQubuCyw39YrjxuSooGLRJ1SKYE5ZY68uJib5ZigI4/edit#heading=h.up2cdet4w24u)
 - [I created and delivered a presentation for the Maintainers about the beta phase](https://docs.google.com/presentation/d/1qA9U4BkLKW_kOn696jKkDbUgv910_i-sGbHTZ9tyURQ/edit?usp=sharing)
 - [{sandpaper} I refactored the aio page and keypoints to use an internal aggregator](https://github.com/carpentries/sandpaper/pull/272)
 - [{sandpaper} I added images and instructor notes aggregators](https://github.com/carpentries/sandpaper/pull/272)
 - [{sandpaper} I updated the package checks](https://github.com/carpentries/sandpaper/pull/275)
 - [{sandpaper} I experimented with setting install-r: false in the install-r github action](https://github.com/zkamvar/feverish-cowbell/commit/a7441db31ff23754efa815876ca9e6cf2ada1193) (more context can be found at https://epiforecasts.io/posts/2022-04-11-robust-actions/index.html)

#### What did you struggle with?

I think I struggled with refactoring, mostly

#### What would you like to work on next week?

 - Develop Beta Phase opt-in forms
 - Write up Beta Phase Blog Post announcing the beta phase
    - contact IDC, Karen, Dan for feedback
 - Update lesson-transition script

#### Where do you need help from François?

AWS setup for beta phase

#### Any other topics

I got the RStudio diversity scholarship and my talk was accepted! Now I just gotta write the thing!

### Date: 2022-04-15

#### Who did you help this week?

 - I helped Danielle with a couple od things
 - I helped David P. understand the scope of suggested changes
 - I helped Christian K. understand the process of updating the lesson.

#### Who helped you this week?

 - Not sure

#### What did you achieve?

 - []()
 - [(actions) I made a quick fix for the changes in the R-universe API](https://github.com/carpentries/actions/commit/64484cf3bfc20c50538018feddec1c05a1400948)
 - [{sandpaper} I added the all in one page](https://github.com/carpentries/sandpaper/pull/271)
 - [(lesson-transition) I created more diagrams that better illustrate the processs](https://github.com/data-lessons/lesson-transition#readme)
 - [{sandpaper} I began refactoring the provisioning of pages like keypoints and aio that use rendered elements](https://github.com/carpentries/sandpaper/compare/0.4.0...common-html)

#### What did you struggle with?

My left middle finger became strained on Wednesday and I had to take half of Thursday off to deal with it. It is difficult to type with nine fingers and the doctor recommended that I rest the finger. 

#### What would you like to work on next week?

 - Review my plan for the month
 - Review my Curriculum Team and Roadmap Plan
 - Document metadata for lessons
 - Write images page

#### Where do you need help from François?

I need to understand if my planning makes any sense or if there are gaps anywhere. 

#### Any other topics

This week wqas a bit ofa tyrain wreck.

### Date: 2022-04-08

#### Who did you help this week?

 - I helped Erin by running the code to reitire maintainers who opted-out of
   maintainership via the survey.
 - I blocked a malicious user from our orgs
 - I set a slack channel that was accidentally public to private
 - I was able to respond to queries from https://github.com/r-devel/r-bug-tracking-lesson

#### Who helped you this week?

 - François helped me by recovering the names of my community discussion participants
 - Kari helped me by taking a look at my plan for the beta phase conversion
 - Sher! helped me by adding me to the IDC agenda

#### What did you achieve?

 - []()
 - [I created a more concrete transition plan including a diagram](https://docs.google.com/document/d/1EMQubuCyw39YrjxuSooGLRJ1SKYE5ZY68uJib5ZigI4/)
 - I ran two community discussions on the workbench
 - [{varnish} I added updates that allow custom engines to show through](https://github.com/carpentries/varnish/releases/tag/0.1.8)
 - [{sandpaper} I updated sandpaper to update with the varnish version](https://github.com/carpentries/sandpaper/releases/tag/0.3.6)
 - [(styles) I reviewd François' transition setup for styles](https://github.com/carpentries/styles/pull/637)

#### What did you struggle with?

I think I struggled a bit with planning the beta phase.

#### What would you like to work on next week?

 - Review my plan for the month
 - Review my Curriculum Team and Roadmap Plan
 - Document metadata for lessons
 - Write images page

#### Where do you need help from François?

I need to understand if my planning makes any sense or if there are gaps anywhere. 

#### Any other topics

It's really nice to see that the project is getting traction outside of our organisation. I'm really glad that the R folks have picked it up and their usage is showing me the gaps in the documentation that I didn't have previously. In a way these are the pre-beta testers. One of the things I'm feeling is that I need to really set a formal way of getting feedback from participants, but I don't have a coherent plan for managing or analysing that right now. I think this might be an area where Kelly or Karen may be able to help, but ultimately I'm not sure. 

### Date: 2022-03-25

#### Who did you help this week?

 - I helped Erin fixing some R code that's been handed down to draw our cumulative impact map, but was broken due to new tags in our system.
 - I also helped Erin by writing API calls to get the team information for each repository
 - I helped Kari by anonymizing the DoF applications
 - I helped folks in the welcome session on Wednesday by providing help with slack. 

#### Who helped you this week?

 - Erin and Françios helped me by reviewing my RStudio submission
 - François helped me by brainstorming deployment ideas for the beta phase
 - Michael helpe me by presenting the results from the LPTF

#### What did you achieve?

 - [{tinkr} fixed a bug that appeared in commonmark 1.8](https://github.com/ropensci/tinkr/pull/67)
 - [(beta phase) I wrote the transition script for the r-socialsci lesson](https://github.com/data-lessons/lesson-transition/commits?author=zkamvar&since=2022-03-21&until=2022-03-26)
 - I submitted my Diversity Scholarship submission
 - I submitted my rstudio::conf(2022) submission
 - I anonymized 34 applications for DoF
 - I wrote a script that identifies the teams per repository for our orgs
 - I tested out a dual-deployment strategy for our lessons in beta phase;
   François and I decided that we should go with a static gh-pages and a
   dynamic beta. We will make changes to the static gh-pages at the end of the
   beta phase
 - François and I wrote up a plan for the beta phase deployment

#### What did you struggle with?

I struggled a bit with prioritizing tasks, but I think I made it out okay in the end.

#### What would you like to work on next week?

Nothing. I will be on Vacation

#### Where do you need help from François?

Communicate to the beta repos

#### Any other topics

Nope: vacation

### Date: 2022-03-18

Note: This comes three weeks after the last update for the following reasons:

Week of the 27th: I worked two days due to moving, mental issues, and a personal holiday. I spoke with Sher! and Danielle about the Instructor community and fixed some things regarding links and workflows in sandpaper. 

Week of the 6th: This was the retreat and I broke my charger on the second day, so I wasn't able to get much accomplished.

#### Who did you help this week?

 - I added context for Alycia's question about licensing to the legal expert questions document
 - I helped Danielle and Daniel Chávez by updating his workshop-es page with the correct survey links and CSS: https://github.com/dechavezv/2022-05-07-Ecuador-PUCE/pull/1
 - I helped myself by taking rest yesterday when I was not in a good mental state

#### Who helped you this week?

 - Erin, Toby, and François reminded me to be kinder to myself when I was feeling like a pile of garbage wrapped in human skin
 - Kari encouraged me to apply to funding from RStudio
 - Michael explained his workflow to me to help me understand why the R-Ecology lesson was not passing checks
 - François helped me figure out a better plan for the beta phase the workbench
 - Toby brainstormed with me about the beta phase and helped me realize that it's better to push things back
 - Erin gave feedback on my RStudio submission

#### What did you achieve?

 - [(actions) I added a pinning mechanism to our actions for sandpaper and varnish](https://github.com/carpentries/actions/pull/40)
 - I demonstrated the workbench to a couple of maintainers at the maintainer meetings. 
 - [{renv} I discovered an issue with renv that prevents our lessons from processing yaml chunk syntax](https://github.com/rstudio/renv/issues/963)
 - I wrote a first draft of my RStudio::conf(2022) submission.

#### What did you struggle with?

Again, I struggled with a lot of things. I had to take a sick day on Thursday to
clear my mental space. (This is unchanged from three weeks ago!)

#### What would you like to work on next week?

* submit RStudio conf talk
* finalize Beta Phase Communication Plan
* re-draft branch of varnish that uses the styles template for testing

#### Where do you need help from François?

Review of the RStudio application and Beta Phase Plan (once it comes out)

#### Any other topics

I just want to reiterate how utterly cool this is: https://sabaferdous12.github.io/lesson2_sandpaper/01-introduction.html

### Date: 2022-02-25

#### Who did you help this week?

 - I helped Maneesha with the welcome session
 - I helped Toby and Sarah by fixing more bugs in the workbench
 - I helped the Toby and the maintainers of the r-socialsci lesson to figure out what to do with extra content for the styles repo

#### Who helped you this week?

 - Toby and Sarah helped me by providing useful feedback on the behavior of the infrastructure
 - Jeroen helped me by confirming that the API for R-Universe changed
 - Toby helped by asking important questions about features that have not yet been implemented and by positing the real benefits of the workbench
 - Aleksandra helped me by showing a desire path that existed for the styles template that is no longer valid in the new infrastructure
 - Aleksandra and Toby helped me by providing feedback on the template mechanism for the infrastructure, making me realise that I could make it easier
 - Omar, Alycia, and Danielle helped me by responding to my queries about communication and organising
 - François helped me by talking through a potential AWS integration.


#### What did you achieve?

 - I spoke with Omar and Alycia about the strategy for lead up and during the beta phase of the workbench. In essence:
   - clearly advertise the sessions in advance of the sessions
   - give people tasks
   - make the beta phase issues easy to spot via github labels
   - focus communication on GitHub and add responders to the other channels notifying people that the response will be slower there
 - I commented on a lot of PRs in the lesson development training repo
 - [{sandpaper} I merged the PR to add the links.md file](https://github.com/carpentries/sandpaper/pull/257)
 - [{sandpaper} I fixed a bug with links and footnotes](https://github.com/carpentries/sandpaper/pull/258)
 - [{pegboard} same as above](https://github.com/carpentries/pegboard/pull/82)
 - [(actions) I fixed a bug due to the R-universe API changes](https://github.com/carpentries/actions/pull/38)
 - [(lesson tranistion) I added three more repositories and maybe figured out submodules](https://github.com/data-lessons/lesson-transition/commits?author=zkamvar&since=2022-02-22&until=2022-02-26)
 - [(Workbench Documentation) I updated the documentation to include links and proper setup](https://github.com/carpentries/sandpaper-docs/commit/f6e52b526b8fe0d4c126ad1ccfe770d621d31eea)
 - []()

#### What did you struggle with?

Again, I struggled with a lot of things. I had to take a sick day on Thursday to
clear my mental space.

#### What would you like to work on next week?

* implement the search bar for the lessons
* implement the AIO page
* finalize beta phase plan
* prepare for the CT retreat skillup

#### Where do you need help from François?

Nowhere at the moment.

#### Any other topics

I just want to reiterate how utterly cool this is: https://sabaferdous12.github.io/lesson2_sandpaper/01-introduction.html

### Date: 2022-02-18

(updated on 2022-02-22)

#### Who did you help this week?

 - I can not remember who I helped. I normally check slack for this, but it is down :/

#### Who helped you this week?

 - Toby and Sarah helped me by providing useful feedback on the behavior of the infrastructure
 - I know I have more, but again... slack is down.

#### What did you achieve?

 - I submitted the UseR! 2022 proposal
 - [{pegboard} I added a validate divs method](https://github.com/carpentries/pegboard/pull/78)
 - [{sandpaper} I integrated validation into the lesson building](https://github.com/carpentries/sandpaper/pull/255)
 - [{sandpaper} Started PR to provide common links.md](https://github.com/carpentries/sandpaper/pull/257)
 - [{sandpaper} fixed a bug from {cli}](https://github.com/carpentries/sandpaper/issues/252)
 - [(RStudio) reported on a bug/feature with updating packages](https://github.com/rstudio/rstudio/issues/2656#issuecomment-1044764917)
 - []()

#### What did you struggle with?

A lot of things. I had to take a half day on Tuesday and then nearly the whole
day on Wednesday due to mental health and lack of internet. After that I was
able to be fairly productive. 

#### What would you like to work on next week?

* implement the search bar for the lessons
* implement the AIO page
* finalize beta phase plan

#### Where do you need help from François?

Nowhere at the moment.

#### Any other topics

Ha! Ha! Slack is down! GitHub is down (in some places)!

### Date: 2022-02-11

#### Who did you help this week?

 - I helped my friend by giving her a place to stay for a couple of days
 - I helped unblur the RStudio logo on our website for Erin
 - I provided a status update for https://github.com/carpentries/strategic-plan/issues/9 for Kari

#### Who helped you this week?

 - François helped silence my paranoia brain this morning when I was thinking about the infrastructure
 - Toby and Sarah helped me by responding to thier Git issues. 
 - François, Erin, Toby, and Michael helped by reviewing my UseR! proposal
 - Karen helped me by giving me context for how she conducted her instructor training update and who I should contact wrt beta testing with the instructors
 - Omar helped me by coming up with really sweet hex stickers

#### What did you achieve?

 - [(Beta Plan) I drafted the initial beta phase plan](https://docs.google.com/document/d/1F3orzvirzsguJDKmU_66DsQRX77PKZw2O4Dc8JzgdTs/edit)
 - [(UseR! 2022 workshop proposal) drafted](https://docs.google.com/document/d/1Ne1eRjRpYlJUHa__H_2DHBTu3gX1yAqaUAyRdV8Rzz4/edit#)
 - [(UseR! 2022 workshop proposal) drafted](https://docs.google.com/document/d/1Ne1eRjRpYlJUHa__H_2DHBTu3gX1yAqaUAyRdV8Rzz4/edit#)
 - [{sandpaper} a WHOLE BUNCHA WORK that simplified the process of building](https://github.com/carpentries/sandpaper/commits?author=zkamvar&since=2022-02-07&until=2022-02-12)
 - Miscellaneous other things that my brain is too tired to remember.

#### What did you struggle with?

Coming to terms with the fact that my code is slow for now. 

#### What would you like to work on next week?

* submit the proposal to UseR! 2022
* implement the search bar for the lessons
* implement the AIO page
* finalize beta phase plan

#### Where do you need help from François?

Nowhere at the moment.

#### Any other topics

Refactoring is hard, but I'm glad I did it. The AIO page should not take too 
much effort to implement. The search bar is an interesting beast because it
works a bit differently than was set up in the bytes.co template. I wrote
it up in a commit here: https://github.com/carpentries/varnish/commit/e61903281c78a3d03ed89f9c3dba2f1a3cd8fbfd.
Effectively, during the design process we never envisioned what the search would
look like from the user's end because right now we have a search bar that points
people to a new page, so that's why people use the AIO page. The pkgdown search
bar implements one that really does not need a button because it generates a
dropdown menu from the search and then it is up to the user to select from that
menu. I can see us being able to implement it either way, but from usage, I get
the feeling that people would much prefer a dynamic search bar (I know I would,
but it's not clear what the a11y implications are [though I know that bootstrap
has some documentation on that]) because that's effectively what they use the 
all in one page for.

### Date: 2022-02-04

#### Who did you help this week?

 - I helped Toby by swapping lab meetings with him when he was feeling a bit
   overwhelemed.
 - I helped the team by anonymizing applications
 - I deleted a SPAM post for Omar
 - I added Toby to the instructor-training repository so that toby could be
   assigned to a task
 - I helped Alycia with editing a blog post on GitHub

#### Who helped you this week?

 - The entire team really helped me by being enthusiastic about The Carpentries Workbench
 - Toby and Michael helped me by explaining that there were a lot of features that I did not show in my demonstration during the lab meeting. 
 - Toby asked a really good question about prioritization of requests from the community
 - Kari asked a really good question about what the next steps are for the rollout
 - Allison Hill posted a link to an effective way to get feedback about a software project
 - Toby and Sarah Stevens pointed out issues that they had with the infrastructure
 - Two community members emailed me telling me that The Workbench was perfect for their needs

#### What did you achieve?

 - [(blog) The Carpentries Workbench blog post was published](https://github.com/carpentries/carpentries.org/pull/1308)
 - [{sandpaper} got four releases](https://github.com/carpentries/sandpaper/releases)
 - [{sandpaper} started refactor of global variables for varnish](https://github.com/carpentries/sandpaper/pull/248)
 - [{varnish} fixed logo; add tracking; update license](https://github.com/carpentries/varnish/releases)
 - [{pegboard} fix a bug in keypoints and update license information](https://github.com/carpentries/pegboard/releases)
 - [(transformation) rebuilt and published most of the test lessons](https://github.com/fishtree-attempt/)
 - [(universe) only publish releases on the universe](https://github.com/carpentries/universe/commit/01fed5509b720d210a8ea5ce1a4b2a0345693077)
 - Presented The Carpentries Workbench at the Core Team meeting
 - Anonymized fifteen applications


#### What did you struggle with?

Refactoring on a Friday :weary:

#### What would you like to work on next week?

* clean up some of the spaghetti code in sandpaper
* plan beta phase with expected feedback and outcomes
* submit the proposal to UseR! 2022

#### Where do you need help from François?

Nowhere at the moment.

#### Any other topics

I had to nap right after the Core Team meeting. I think I've been doing so much
deep work that being in the spotlight is a bit uncomfortable and slightly
exhausting. The refactoring that I tried to tackle this week is important work
because it will make things easier for us to pivot when new things need to be
added or the build system needs to change. 

### Date: 2022-01-28

#### Who did you help this week?

 - I helped Toby by telling him about my plans for the credits page
 - I helped Annajiat by telling him about our perspectives and resources for i18n
 - I helped a lesson developer by pointing to resources for including math in the lessons
 - I helped a community member by pointing out a fix for the raster package isntallation issues

#### Who helped you this week?

 - François, Maneesha, and Talisha helped me by clarifying license language
 - The entire Curriculum Development Team helped me by brainstorming on ways I could run community discussions
 - François helped me by discussing my plans and how my work fit in with our Grants and Strategic Plan
 - Toby, François, Omar, and Alycia helped me by reviewing my blog post
 - Danielle Navarro gave me permission to use the title "workbench" for our infrastructure.

#### What did you achieve?

 - [(blog) I wrote a blog post about The Carpentries Workbench](https://carpentries.org/blog/2022/01/live-lesson-infrastructure/)
 - [{sandpaper} ](https://github.com/carpentries/sandpaper/commits?author=zkamvar&since=2022-01-24&until=2022-01-29)
 - [{varnish} fixed some visual elements; add blockquotes; update footer; update readme](https://github.com/carpentries/varnish/commits?author=zkamvar&since=2022-01-24&until=2022-01-29)
 - [(documentation) update documentation for The Workbench](https://github.com/carpentries/sandpaper-docs/commits?author=zkamvar&since=2022-01-24&until=2022-01-29)
 - Created two templates for the lessons created via the Workbench: https://github.com/carpentries/workbench-template-rmd and https://github.com/carpentries/workbench-template-md
 - [(actions) speed up the provisioning of R packages for R-based lessons](https://github.com/carpentries/actions/commits?author=zkamvar&since=2022-01-24&until=2022-01-29)

#### What did you struggle with?

I can not remember to be honest. 

#### What would you like to work on next week?

* fix an error in varnish that is causing the assets folder to be ignored in some contexts
* clean up some of the spaghetti code in sandpaper

#### Where do you need help from François?

Still relevant!

* Please clone the sandpaper documentation site and then do two things:
   1. build it with the current version of sandpaper and varnish
   2. install the pull requests on sandpaper and varnish and then build it again
      (though be aware that I need to add a catch that invalidates a part of the
      cache, but I'm le tired and can't remember what it is)

#### Any other topics

This was another heavy week, but I'm proud of the work that I did. It feels like
a lot of work and only a little bit of work at the same time, IDK, it's weird. 
I still fear that folks will complain about how slow the infrastructure is, but
I just need to remember that we will speed it up in the end. 

### Date: 2022-01-21

#### Who did you help this week?

 - I helped Toby get started with his lesson
 - I helped Michael by fixing an RMarkdown rendering error
 - I helped Dan by taking notes at the Maintainer Meeting
 - I helped Omar be reassuring him that it was absolutely no problem to not have
   the sticker designs finished by this week. 

#### Who helped you this week?

 - Toby helped me by being up for and positive about testing out the new
   infrastructure. There were a couple of bumps, but nothing that he nor I
   could not get over
 - Dan helped me by doing a bang-up job of running the maintainer meetings.

#### What did you achieve?

 - added the instructor view to the lessons
 - [debugged an odd behavior with pandoc 2.17](https://github.com/jgm/pandoc/issues/7843)
 - added navigational elements into the new frontend
 - added some basic metadata generation to the lessons, which I have 
   demonstrated working in the [R Ecology Lesson in the fishtree-attempt
   repo](https://validator.schema.org/#url=https%3A%2F%2Ffishtree-attempt.github.io%2FR-ecology-lesson%2F04-visualization-ggplot2.html)
 - migrated the building of the JS/CSS over to varnish
 - wrote some new tests for the infrastructure (but still need to write more)

#### What did you struggle with?

The Lua filters were throwing me for a loop plus the fact that the builds are
now slower messed with my self-confidence a bit, but it will be added value when
I make changes that automatically speed up the infrastructure. 

#### What would you like to work on next week?

* fix how our github actions installs lesson dependencies. 
* add CITATION.cff file to lesson tempalte for metadata
* release sandpaper and varnish 0.1.0
* write the blog post and show off

#### Where do you need help from François?

* Please clone the sandpaper documentation site and then do two things:
   1. build it with the current version of sandpaper and varnish
   2. install the pull requests on sandpaper and varnish and then build it again
      (though be aware that I need to add a catch that invalidates a part of the
      cache, but I'm le tired and can't remember what it is)

#### Any other topics

We close on our house next week and thus I am dealing with all sortsa stress rn.
The lesson is coming along, its still a bit rusty and demonstrating it is not
very nice because there is a delay between when you save a file and it builds
on the screen (~3-4 seconds), but it _does_ work. 

My coach mentioned that I need to sit down and really take a look from the top
down about how my work fits in with the strategic plan because at the moment, I
am working in a very task-based manner that is causing a lot of anxiety. I'm 
going to try to accomplish this during the next R&R day. 


### Date: 2022-01-14

#### Who did you help this week?

 - I helped François by taking notes at the CT meeting
 - I helped Alycia by asking relevant questions at the data Sovereignty meeting.

#### Who helped you this week?

 - Alycia and Toby helped me by providing good context and followups for the
   Data Sovereignty meeting.
 - Kari helped me by asking specifics about the plans for the new
   infrastructure rollout in relation to instructors

#### What did you achieve?

I have gotten _very_ close to releasing the new version of sandpaper and
varnish (the engine and the styling, respectively). The only hangups right now
are issues around failing tests on windows with pandoc. This project has taken 
up the vast majority of my time aside from meetings.

#### What did you struggle with?

Pandoc Lua filters and random css/javascript funkiness

#### What would you like to work on next week?

* add the appropriate links and navbar for the lesson
* add CITATION.cff file to lesson tempalte for metadata
* release sandpaper and varnish 0.1.0

#### Where do you need help from François?

* nowhere at the moment

#### Any other topics

I am excited for the new changes and one of the things that's currently dragging
me down is the fact that it takes 10 minutes for the CI to run through the 
checks. It's something that I'm aware of and there's not much I can do about it
right now. The thing that's making my life difficult is testing on Windows
because it uses the nightly builds of pandoc, but there are changes in the lua
filters that are causing my old filters to break, which is partially because I 
only _kinda_ know what the heck I'm doing with them. The last error gave me line
numbers, so I can definitely work with that next time I pick it up on Monday.

### Date: 2022-01-07

#### Who did you help this week?

 - I helped Michael with technical support for the new infrastructure
 - I helped a community member by fixing a bug on Windows

#### Who helped you this week?

 - Alycia helped me by providing me ample context for our meeting regarding CARE principles next week
 - Toby helped me by succinctly explaining our plan for the metadata on our lessons
 - François helped me by reminding me about the CZI grant deliverables so that I could prioritize my work

#### What did you achieve?

 - [{sandpaper} fixed a bug coming from the new version of {renv}](https://github.com/carpentries/sandpaper/pull/225)
 - [{sandpaper} fixed a bug with lua filters](https://github.com/carpentries/sandpaper/pull/226)
 - [{actions} made the lesson dependencies respect github packages and simplify](https://github.com/carpentries/actions/pull/35)
 - [{pegboard} fixed a bug on windows if the user's library had spaces in the path](https://github.com/carpentries/pegboard/pull/73)
 - [tested and explored new frontend](https://zkamvar.github.io/shellac/student_carpentries.html)
 - Had a meeting with the people from Zenodo regarding metadata
 - Drafted 3 month roadmap for the lesson infrastructure

#### What did you struggle with?

Trying to find a fix and a test for a windows error was definitely challenging,
but I think some of the most challenging things have been trying to come up
with a succinct way to fit the framework of the new frontend into our existing
framework. I've had to fix a couple of minor mistakes from the code, but there
are additional things that I should add to make sure that the new lessons have
pairity with the old lessons. A salient example is code highlighting, which 
pandoc does via spans, but this was not provided during the design or the coding.
When we asked the coding contractor about it, they mentioned how this method 
may be problematic, but did not give a specific example of how it was so.

There is also the idea of how should I properly add or modify the work from the
contractors? They worked with it and did all the testing to make sure that it is
up to WCAG AA standards, so how do I know that I can modify it to suit our build
process? 

#### What would you like to work on next week?


* setup the new frontend to work for our lessons
* add CITATION.cff file to lesson tempalte for metadata

#### Where do you need help from François?

* nowhere at the moment

#### Any other topics

I think I acatually put all of this in the "what did you struggle with" section

