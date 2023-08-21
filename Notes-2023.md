f Meeting Notes

## Table of Contents

 - [2023-08-18](#date-2023-08-18)
 - [2023-08-11](#date-2023-08-11)
 - [2023-08-04](#date-2023-08-04)
 - [2023-07-28](#date-2023-07-28)
 - [2023-07-24](#date-2023-07-24)
 - [2023-07-14](#date-2023-07-14)
 - [2023-06-16](#date-2023-06-16)
 - [2023-05-26](#date-2023-05-26)
 - [2023-05-19](#date-2023-05-19)
 - [2023-05-10](#date-2023-05-10)
 - [2023-04-21](#date-2023-04-21)
 - [2023-04-14](#date-2023-04-14)
 - [2023-04-07](#date-2023-04-07)
 - [2023-03-31](#date-2023-03-31)
 - [2023-03-25](#date-2023-03-25)
 - [2023-03-17](#date-2023-03-17)
 - [2023-03-10](#date-2023-03-10)
 - [2023-02-17](#date-2023-02-17)
 - [2023-02-09](#date-2023-02-09)
 - [2023-01-27](#date-2023-01-27)
 - [2023-01-20](#date-2023-01-20)
 - [2023-01-13](#date-2023-01-13)
 - [2023-01-06](#date-2023-01-06)

### Date: 2023-08-18

This week was a half week as I had vacation for two days and took sick leave for
part of Monday.

#### Who did you help this week?
 
 - Kelly needed an idea of what to look for regarding specs for a new computer. 
   I recommended she get a Dell XPS because they all come with at least 8G of
   ram and > 1.3 GHz processor. 

#### Who helped you this week?

 - Toby Hodges provided a community member some context for lack of accurate
   timings in the R Ecology Lesson episodes (they used the `minutes` keyword).
 - Toby and Rob made some progress with the spoiler class
 - Toby reminded me that I can assign documentation related issues to him

#### What did you achieve?

 - Opened PRs to fix a couple of things in {varnish}
   - [fix overeager mathjax formatting weirdness](https://github.com/carpentries/varnish/pull/90)
   - [(draft) fix problem with bold italic text being clobbered by default font weight](https://github.com/carpentries/varnish/pull/91)
 - Drafted PR to account for child files in {sandpaper}
   - source: Incubator lesson [manging-computational-projects#103](https://github.com/carpentries-incubator/managing-computational-projects/issues/103)
   - Managed expectations WRT request overload on the issue: [carpentries/sandpdpaper#497](https://github.com/carpentries/sandpaper/issues/497)
   - [PR carpentries/sandpaper#499](https://github.com/carpentries/sandpaper/pull/499)
   - Live-coded problem solving for this issue: <https://youtu.be/k1pM7QyVc0g?si=aaEQKK39I5aCfV6M>
 - Found [{sandpaper} issue related to 404 page with nested links](https://github.com/carpentries/sandpaper/issues/498)
 - Encountered frustration with {renv}: <https://github.com/carpentries/sandpaper/issues/500>

#### What did you struggle with?

I didn't attend the maintainer meeting because I had forgotten to tell Erin to
fill in when I was out, so the maintainers in the Pacific time meeting were
left wondering where everyone was. 

#### What would you like to work on next week?

Below is from two weeks ago and still relevant, but I would like to finalize the
overview lesson structures for testing, because the deadline for that is  coming
up.

I would like to write a vignette that describes how {pegboard} structures the
lesson data and what you can use it for. I would also like to document 
{pegboard}'s philosophy a bit more and the debugging strategy that I showed.

Of course I want to expand more on the update workflow philosophy and the pull
request workflow philosophy. If I have time, I would also like to get more 
progress with the search bar. 

#### Where do you need help from Rob?

Let me know if you are doing okay. 

#### What did you learn this week?

Not sure.

#### Anything else?

I would really like to figure out exactly how to assign review tasks for The
Workbench. You told me to tag you if I need anything reviewed and I do tag the
Workbench Maintainer group, but I think this is a situation where no one wants
to raise their hand to provide a review, so the PRs remain up for more than a
week and then they become overwhelming for me. It's important to me that we
start getting into the habit of these because I want to make sure that y'all
have some organisation beyond "lol this looks good whatevz," but I really do not
know how to have this discussion. 

### Date: 2023-08-11

This week was very much spent on working with workshop overview sites. I also
gave my first stream doing debugging.

#### Who did you help this week?

 - provided guidance for someone setting up a workshop website
 - provided guidance for a learner asking about setting up Notepad++ as the default editor on Windows (pointed to issues page)
 - Simon Christ by providing context for transitioning his lesson to the workbench
 - Erin by explaining the confusing situation that happened with the maintainer
   groups. 
 - Helped maintainers of geospatial-python with [post-transition woes](https://github.com/carpentries/workbench/issues/66)


#### Who helped you this week?

 - Erin reviewed and merged the pegboard PR that was sitting there for a few days
 - Toby validated my frustration about a GitHub comment from a community member that restated the obvious.

#### What did you achieve?

 - I opened a trio of pull requests to enable workshop overview lessons (see [workbench#65](https://github.com/carpentries/workbench/issues/65) for details)
   - [pegboard#132](https://github.com/carpentries/pegboard/pull/132) to allow the validator to parse with no episodes
   - [varnish#87](https://github.com/carpentries/varnish/pull/87) adds overview template; updates css and js to properly hide sidebar in an overview page
   - [sandpaper#496](https://github.com/carpentries/sandpaper/pull/496) processes overview lessons without episodes 
   - [lesson-transition#92](https://github.com/carpentries/lesson-transition/pull/92) test transition workflow for overview lessons
 - I live streamed my coding of the above on Wednesday and [saved it to YouTube as an Unlisted playlist](https://www.youtube.com/playlist?list=PLSFzyC3wp8-dRdph8bqBkSM81lDplH9B5) 


#### What did you struggle with?

I struggled with the overview lesson tasks. One of the things I'm struggling
with is how the sidebar is handled in the website while switching between
desktop and mobile views. In mobile view, the sidebar and the navbar contain
the same content, but in desktop view, they contain different content and it's
frustrating to try to manipulate the sidebar not knowing if it will retain the
a11y properties for overview lessons. I think the solution I've come up with for
the overview lessons _works_, but I'm still beating myself up for not explicitly
taking care of those earlier.

#### What would you like to work on next week?

Below is from last week and still relevant, but I would like to finalize the
overview lesson structures for testing.

I would like to write a vignette that describes how {pegboard} structures the
lesson data and what you can use it for. I would also like to document 
{pegboard}'s philosophy a bit more and the debugging strategy that I showed.

Of course I want to expand more on the update workflow philosophy and the pull
request workflow philosophy. If I have time, I would also like to get more 
progress with the search bar. 

#### Where do you need help from Rob?

Let me know if you are doing okay. 

#### What did you learn this week?

Not sure.

#### Anything else?

Nope

### Date: 2023-08-04


It's been a week. I got a bit flustered in the middle and ended up being a bit
of a pill to people until Wednesday. Things got better on Thursday and Friday.

#### Who did you help this week?

 - clarified for Maneesha the status of the search bar
 - helped myself by removing the damn zapier integration for workbench issues
   going to Asana. They were frustrating me because they just kept piling up for
   every issue and pull request and just made it so that I was tracking them in
   both GitHub and asana, which was a fucking nightmare (not like the one I woke
   up from screaming on Wednesday evening, which felt more like it was directed
   by David Lynch.... and it was _far_ better than being in Asana). 
 - provided guidance for Alycia to not respond to a weird unprompted tweet
   asking if we were considering using markdown slides because it smelled an
   awful lot like [\#BropenScience](https://www.bps.org.uk/psychologist/bropenscience-broken-science).
 - helped Simon C. as best as I could with the transition workflow.
 - pointed Toby towards a link to the solution to the "buoyancy" of the
   solution blocks in The Workbench

#### Who helped you this week?

 - Toby added documentation to sandpaper-docs about the cure for the floating 
   solutions
 - Maneesha got me to get my ass off the floor and prototype a search bar (I
   did not spend too much time on this; ~3 hours).
 - Erin added clarification to the episode structure episode
 - Rob was understanding as I was wearing my nits end on Tuesday and Wednesday.
 - Toby shared with me a testimonial that Malvika wrote about The Workbench.

#### What did you achieve?

This week was actually kinda productive. I got a bit of documentation done, 
debugged some {renv} issues, and tracked some workbench bugs.

 - (lesson-transition) [Reviewed and merged Toby's contribution for the good-enough-practices lesson](https://github.com/carpentries/lesson-transition/pull/90)
 - (lesson-transition) [Made a lot of commits to address the {renv} debacle slowing the builds down](https://github.com/carpentries/lesson-transition/commits?author=zkamvar&since=2023-08-01&until=2023-08-05)
 - (lesson-transition) [Reset the transition test repository](https://github.com/fishtree-attempt/znk-transition-test)
   - {renv} [made a bit of noise on a bug that I was also experiencing](https://github.com/rstudio/renv/issues/1617)
 - {vise} [refactored update reporter to work with renv > 1.0.0](https://github.com/carpentries/vise/pull/6)
   - {renv} [found a bug that was preventing {vise} from being loaded](https://github.com/rstudio/renv/issues/1621)
 - (developer documentation) Populated the [Remote Workflows Chapter](https://carpentries.github.io/workbench-dev/remote/intro.html)
   - Created [script to demonstrate platform-independent deploy](https://carpentries.github.io/workbench-dev/remote/intro.html#proof)
   - Began [description/philosophy and requirements for
     deployment](https://carpentries.github.io/workbench-dev/remote/deploy.html)
     (this includes things like how the caching works and why we chose the
     toolse we chose.
 - {pegboard} demonstrated and recored [error Simon C. found if an HTML image was inside an HTML comment](https://github.com/carpentries/pegboard/issues/130)
   - {pegboard} created [pull request to fix html images embedded in comments](https://github.com/carpentries/pegboard/pull/131)
 - {sandpaper}/{varnish} prototype search functionality: <https://zkamvar.github.io/instructor-training/>
   - {varnish} [adapted HTML, CSS, and JS from {pkgdown}](https://github.com/carpentries/varnish/pull/86) (this is where the journey of debugging is recorded)
   - {sandpaper} [enabled search by updating metadata and using pkgdown indexer](https://github.com/carpentries/sandpaper/pull/495/files)

#### What did you struggle with?

I struggled a lot with trying to compartmentalize the pressure that I was feeling.
I saw that Toby was moving forward with advising the soon-to-be lab maintainers
on the procedure for the lesson transition workflow and panicked a bit. The 
{renv} package update builds failed, but I don't want to have them run, because
they will update to version 1.0.0, which has a lot of problems. I want to make
a better catch for its problems, but not much time to separate it out from 
{sandpaper} neatly. On top of that, I was asked yet again about the search bar.
It's one of those sore points because it existed in our lessons, but it just 
went to google, so people didn't really use it much, so that's why we didn't 
implement it earlier, but now the fact that it's disabled is making people 
more aware of it.

#### What would you like to work on next week?

I would like to write a vignette that describes how {pegboard} structures the
lesson data and what you can use it for. I would also like to document 
{pegboard}'s philosophy a bit more and the debugging strategy that I showed.

Of course I want to expand more on the update workflow philosophy and the pull
request workflow philosophy. If I have time, I would also like to get more 
progress with the search bar. 

#### Where do you need help from Rob?

Please read <https://carpentries.github.io/workbench-dev/remote/intro.html> and
the following chapter and _try out the script_.

#### What did you learn this week?

Sometimes, it's okay to say fuck it and do the thing you've been wanting to do
for a while.

#### Anything else?

I'm sorry for being short with you on Wednesday. I definitely wasn't in my best
form and I promise that the coworking sessions will be better from now on.

### Date: 2023-07-28

#### Who did you help this week?

 - Erin by addressing the pull requests and orphan branches in the template
   repositories that was causing her confusion.
 - (not sure it was really helping) Eli and Maneesha by linking the varnish 
   colour scheme in the amy-development channel when they were having the BS5
   discussion about contrast.
 - Toby by cementing the maintainers for the image-processing lesson. 

#### Who helped you this week?

 - Alycia made a note to talk with the IDS group to see if they needed extra
   attention with their lesson.
 - Toby by volunteering to do PR work updating the workshop template

#### What did you achieve?

This week felt like a bit of a quiet week partially because I had a day off, a
half a day sick, and a day for professional development. 

 - Started the [remote workflow chapter](https://carpentries.github.io/workbench-dev/remote/intro.html) in the workbench-dev guide (faaaaar from finished) because the documentation for the workflows lives [inside of sandpaper](https://github.com/carpentries/sandpaper/tree/main/inst/workflows#readme).
 - {sandpaper}: [modified the examples to run faster](https://github.com/carpentries/sandpaper/pull/494)
 - {sandpaper}: fixed discussion list link that's been borked for a while now
 - merged old pull requests in the templates: [workbench-template-md#29](https://github.com/carpentries/workbench-template-md/pull/29) and [workbench-template-md#31](https://github.com/carpentries/workbench-template-md/pull/31)
 - PD: wrote a [blog post about how we use the R-universe](https://zkamvar.netlify.app/blog/r-universe-and-cran/) (it will cross-post to rOpenSci next week)
 - PD: finished and submitted application for Fred Hutch job. 


#### What did you struggle with?

Prioritization and organization. It's been a goofy week. 

#### What would you like to work on next week?

Documenting the remote workflows

#### Where do you need help from Rob?

See if you can run this workflow locally with an incubator lesson that has not
been transitioned: https://github.com/carpentries/lesson-transition/blob/main/transition-workflow.md

#### What did you learn this week?

The {flow} package has a neat trick to see the function tree for all the
functions that use a particular function. 

#### Anything else?

nope.

### Date: 2023-07-24

Note: This is 10 days after the last update and I have had to take sick time and
am not in the best of states, so my contributions are low. 

#### Who did you help this week?

 - Kelly by getting the bones of her package set up
 - Erin by coworking on her project and helping her write a function to solve a
   common problem
 - Not sure who else.


#### Who helped you this week?

 - The team for being supportive as I had to take off work to take care of my mother

#### What did you achieve?

 - added more stuff on [the design principles of the package cache](https://carpentries.github.io/workbench-dev/sandpaper/package-cache.html#design-principles)
 - I spent a good chunk of time diagnosing an upstream error in curl that was
   causing R lesson builds to fail: <https://carpentries.github.io/workbench-dev/flight-rules.html#ssl-error>
 - [opened pr to upgrade pandoc in tests](https://github.com/carpentries/sandpaper/pull/492)
 - [approved Erin's PR to update DESCRiPTION in pegboard](https://github.com/carpentries/pegboard/pull/129)
 - [addressed an issue with a lesson using child documents](https://github.com/carpentries-incubator/managing-computational-projects/pull/100)
 - submitted job application for Berkeley RSE position

#### What did you struggle with?

Trying to juggle all the priorities that I have, but things are looking brighter.

#### What would you like to work on next week?

 - Add more use-cases for the flight rules
 - Begin work on allowing the workshop webpages

#### Where do you need help from Rob?

See if you can run this workflow locally with an incubator lesson that has not
been transitioned: https://github.com/carpentries/lesson-transition/blob/main/transition-workflow.md

#### What did you learn this week?

That coworking and pair programming is a valuable tool for getting people onboarded and comfortable with working in a codebase.

#### Anything else?

I'm not actually sure these are being read, so I will send you a reminder about that. 

### Date: 2023-07-14

Note: This is nearly a full month after the last update. I had some days of
vacation in that time, but overall, this last month has been very difficult
mentally and I don't think I was very productive.

#### Who did you help this month?

 - I would _like_ to think that I helped Erin, Kari, and Rob by proposing to
   have the meeting to discuss my thoughts about the communication challenges,
   but it was quite heavy. 


#### Who helped you this month?

 - Liz Stokes, Maëlle Salmon, Rich FitzJohn, Athanasia Mownickel, Malvika
   Sharan, and others have reached out to offer support and connect
   opportunities as they come up.
 - Oscar and Alycia reviewed the blog post and helped me provide important
   details and clarifications.
 - Talisha for checking in with me when I was feeling low about the situation
 - Erin and Rob for sitting with me and having a difficult conversation about 
   the situation that arose due to the lack of specific policy around
   communications about downsizing.
 - Alycia for reminding me about the Core Team meeting that I ended up being
   super late to (and subsequently missed the part that I could have given
   input in).
 - Hao Ye scheduled a meeting with me where I had the opportunity to talk about
   the big picture of lesson infrastructure development and the challenges 
   associated.
 - Kevin Ushy for taking the time to explain processes in {renv} for me
 - Toby for his words of encouragement on my teaching style

#### What did you achieve?

I did a lot of things that felt useful this month and a lot of things that did
not feel so useful. Here are the useful bits:

 - Wrote a lot in [The Workbench Developer's Guide](https://carpentries.github.io/workbench-dev)
 - [{sandpaper} fixed a bunch of tests with {renv} and R-devel](https://github.com/carpentries/sandpaper/commits?author=zkamvar&since=2023-06-17&until=2023-07-15)
 - [{renv} reported an issue with `renv::restore()` in version 1.0.0](https://github.com/rstudio/renv/issues/1544)
   - [sandpaper issue on `manage_deps()`](https://github.com/carpentries/sandpaper/issues/490) (first opened)
   - [sandpaper issue on `update_cache()`](https://github.com/carpentries/sandpaper/issues/491)
   - [created minimal reproducible example](https://github.com/zkamvar/sandpaper-issue-490/#readme)
   - [created reproducible example with lesson](https://github.com/carpentries/sandpaper/issues/490#issuecomment-1632786519) to figure out the dynamics with {sandpaper}
 - [Update internal links section of the workbench documentation](https://github.com/carpentries/sandpaper-docs/commit/68dce22431e3ce58667dc489623695df22e719d7)
 - Wrote and published the blog post for my departure. 

#### What did you struggle with?

Trying to juggle all the priorities that I have, but things are looking brighter.

#### What would you like to work on next week?

 - Cowork with Kelly on Workbench Maintenance
 - Cowork with Maëlle Salmon on tinkr maintenance
 - Get first draft of package cache section done
 - Draft application for UC Berkeley Job

#### Where do you need help from Rob?

See if you can run this workflow locally with an incubator lesson that has not
been transitioned: https://github.com/carpentries/lesson-transition/blob/main/transition-workflow.md

#### What did you learn this month?

That the community truely values my work. 

#### Anything else?

I've been thinking about the policy for letting people go due to budgeting
constraints and I think about the quotes from other non-profits that giving any
more than a month notice for people to be let go is really bad for morale. Erin
said that she is now beginning to understand what that means, but I have another
take on it. I think a lot of nonprofits do good work, but they _do not_ share
our values and I would take their advice with a grain of salt.

The context for giving one month notice I believe comes from the extractive
capitalist nature of most non-profits in which they extract as much work as
possible from their workers without ownership from a clear top-down hierarchy of
programmatic decisions. A one month notice in that situation would shift the
burden of work so rapidly that the remaining workers would not have time to
process what happened to their colleague, so it provides a kind of hard reset.
It represents the _bare minimum_ of policy in a country so dedicated to
squashing labour movements that it doesn't even recognize international labor
day.

I think Erin was absolutely right to push for a long period of notification
because the alternative (one month; no severance) would be a _far worse
situation_, especially given the amount of work that I need to do to ensure
that maintenance of The Workbench runs smoothly after I'm gone and the features
we promised are implemented. If I had been working under the continued
assumption that my funding would remain secure, I would be focused on planning
future improvements to The Workbench with only a minor emphasis on maintenance
from an R package developer's perspective. There really would not have been any
way to have me lead an R package learning group without alerting me to the
funding cliff.

When I brought this up in our meeting about the lack of policy, you mentioned
that it was something that should have been brought up in a contract
negotiation, but here's the thing: I've not been working under a contract since
September 2021, when my initial contract expired. I know that the ET want to
protect people from the concept that their funding may be tenuous, but not
discussing severance policy is akin to denial and leads to my situation. If I
_had_ a contract in place, then it would be a fair assessment to say that it
should have been in there.

I was massively upset because the timing of the communication came on the heels
of me nearly burning myself out trying to get the transition finished and I felt
unappreciated. I do think, however, that the 6 month notice is a good thing
because it gives me the chance to tear down the silo I've been working in and
to strengthen the relationships between the core team members who are tasked
with maintaining The Workbench. The Workbench Learning Group has been pretty
good so far and I can see the connections forming in your heads! The six month
notice (or better yet, 5 months with 1 month severance) is much more likely to
result in a good work environment rather than a 1 month notice.

I truely believe that we have a really special workplace here that does not
suffer the downsides of many other non-profits. We have a strong culture of
honesty, equity, and fairness. I hope that whatever policy is created from this
situation, that it does not go for the low bar. 

### Date: 2023-06-16

Note: this is the week after the core team retreat.

#### Who did you help this week?

 - I may have anti-helped a lot of people on the Core Team :grimace:
 - a community member by fixing a borked etherpad due to an auto-translation
 - Toby, by providing more context for him to create the initial style guide for
   lessons.
 - Jake S by pointing them to https://carpentries.github.io/workbench/faq.html#github-forks 
 - Angelique and Kari by merging https://github.com/carpentries/carpentries.org/pull/1646
 - Sarah Stevens by helping her get a fork set up to deploy to gh-pages
 - Talisha by answering a question about how to nicely display a preview of a changed site so it displayed nicely.

#### Who helped you this week?

 - Is it cheating to say the whole team? It's been a struggle the past month
   and I have mixed feelings (spoonerism: fixed mealings, which sounds like a
   euphamism for diet) about how the announcement of my departure went, but on
   the whole, I feel more connected with my team and I am confident that I will
   still be able to enjoy the next six months even though I will be experiencing
   a high degree of stress.

#### What did you achieve?

I realize I can copy/paste pretty the paragraph from my last update:

This week started and ended with chaos. I'm really looking forward to moving
forward with my situation and being able to be public with it because it's hard
af to pretend everything is fine. That being said, this week was about
documentation, transferring things, and moving slowly. 

Thus, it doesn't seem like I got a lot accomplished: 

 - Transition phase: I rewrote the blog post announcing the workbench transition
   milestone and my own transition news using my voice. 
 - Infrastructure: [added comment identifying use of third party docker container for certbot](https://github.com/carpentries/systems/issues/184#issuecomment-1587398984)
 - Workbench Development Training
   - [added Linux instructions for setup](https://carpentries.github.io/workbench-dev/setup.html#r-packages)
   - [added design and background to the varnish package](https://carpentries.github.io/workbench-dev/varnish/intro.html)
   - Worked with Toby to create first outline and discussion for the Workbench Development Training group
 - (carpentries/actions): added commit and [comment updating the fallout of the change from RStudio -> posit](https://github.com/carpentries/actions/issues/74#issuecomment-1594713466)
   - [Opened issues in our four repositories that use R
     Markdown](https://github.com/datacarpentry/genomics-r-intro/issues/217)
     that they should run the update package cache action.
 - {sandpaper}: fixed an [issue with template page permissions](https://github.com/carpentries/sandpaper/pull/482)


#### What did you struggle with?

Literally everything. I boarded the struggle bus and it got a flat 20 miles out
of town. It was raining and I couldn't get a struggle taxi because there were
others who needed it more than I did, so I struggle walked.

Like, the only things I didn't struggle with was the aspect of my job where I
was trying to develop the documentation and training materials. I developed an
ocular migraine on Monday due to stress and had to have two therapist
appointments this week.

#### What would you like to work on next week?

 - Document the testing workflows and extra packages/actions
 - Organize and triage bugs for The Workbench
 - This is not going to happen; no funds; no time; no energy ~~submit talk for US RSE~~

#### Where do you need help from Rob?

I have not updated my job plan for this quarter because I've spent the majority
of the time preparing and executing the transition. I will do my best to update
it before our next meeting, but likely, I will need to spend time during our
next meeting to complete it.

#### What did you learn this week?

I knew this already but intentions do not make reactions. My actions had caused
a pretty big disruption and people were upset as a result. It was not my
intention, but that's what happened. I learned that I need to just move
forward and focus on progress.

### Date: 2023-05-26

This week was a short week, so there's not going to be much of an entry here.

#### Who did you help this week?

 - Karen by clarifying the process for moving forward with a pull
   request she created on behalf of someone else
 - No one else

#### Who helped you this week?

 - Rob, Toby, and Milan Malfait by creating a solution for chaos that happened
   due to an update with posit: https://github.com/carpentries/actions/pull/75
 - Danielle and Karen helped my by answering my panicky Friday afternoon question

#### What did you achieve?

My vacation was mostly relaxing. We were going to go camping, but there was
still a bunch of snow at the campsite, so we couldn't go.

This week started and ended with chaos. I'm really looking forward to moving
forward with my situation and being able to be public with it because it's hard
af to pretend everything is fine. That being said, this week was about
documentation, transferring things, and moving slowly. 


 - Migrated two resources to The Carpentries organisation
   - [workbench-integration-test](https://github.com/carpentries/workbench-integration-test)
     allows me to test development versions of sandpaper and varnish on live
     lessons.
   - [vise](https://github.com/carpentries/vise) a small package that is used to
     provision the packages used in our GitHub actions. This is mainly used to
     provision the apt packages needed because that is forever a pain in R for
     Linux.
 - Started providing mid-level view of The Workbench workflow from a package
   perspective in [a single broad workflow
   diagram](https://carpentries.github.io/workbench/contributor/#workflows) and
   several smaller [flow
   diagrams](https://carpentries.github.io/workbench/contributor/flow.html)
 - Added [CONTRIBUTING.md to the actions repository](https://github.com/carpentries/actions/pull/78)
 - Reviewed [Toby's update to the Workbench Template](https://github.com/carpentries/workbench-template-rmd/pull/44)
 - [{varnish} finally merge Ben's PR](https://github.com/carpentries/varnish/pull/82)
 - [{sandpaper} fix episode number in sidebar so that it does not disappear](https://github.com/carpentries/sandpaper/pull/472)
   - I'm super not happy with this. The sidebar is a frustrating point in the
     infrastrucutre because it relies on global environment variables and
     awkwardly parsing HTML. I believe I will be able to fix these issues as I
     document the infrastructure, but it's... embarassing.
 - [{sandpaper} detected another weird git user config issue](https://github.com/carpentries-incubator/statistical-probabilistic-programming-r/issues/1)
 - [{renv} detected issue with devel version that is only applicable to really early sandpaper lessons](https://github.com/rstudio/renv/issues/1353)
 - Infrastructure: [fixed Airtable API key for the help-wanted-issues](https://github.com/carpentries/feeds.carpentries.org/issues/78)

#### What did you struggle with?

I struggled a lot with maintaining my self-esteem when I had to implement
https://github.com/carpentries/sandpaper/pull/472. It was frustrating that it
was not obvious _how_ to fix the problem and that the test suite took a minute
to run each time. I struggled even further because of the renv issue and the git
issue above. I struggled because of the looming issue list in sandpaper and the
workbench and for not being able to give satisfactory answers to problems.


#### What would you like to work on next week?

 - Document the testing workflows and extra packages/actions
 - Organize and triage bugs for The Workbench
 - submit talk for US RSE
 - for the future
   - work on {tinkr} updates to parse in-chunk options
   - work on code handout

#### Where do you need help from (T|R)ob(y)?\?


#### What did you learn this week?

I learned that there are a lot of non-obvious things in The Workbench that I
need to make more obvious before the thing happens.

### Date: 2023-05-19

#### Who did you help this week?

 - not sure. I got distracted a bit

#### Who helped you this week?

 - Erin, Alycia, and Rob reviewed my FOSSY 2023 submission
 - Rob made time to sit down with me to talk about the future

#### What did you achieve?

This week overall was a bit of a drag for reasons that are obvious to my dear
readers. It's hard to recall exactly what was done. I submitted my FOSSY talk,
I gave a lab meeting about 2FA, I fixed a bunch of things in {sandpaper} and
fielded a bunch more issues in The Workbench. I pushed back the dovetail blog
post for reasons. Next week is going to be a Napoleonic week for me.

 - I transferred [workbench-integration-test](https://github.com/carpentries/workbench-integration-test) to The Carpentries Org
 - [{sandpaper} 0.12.0 released](https://github.com/carpentries/sandpaper/releases/tag/0.12.0) :ghost: on a FRIDAY :skull:
   - inline images now process correctly 
   - any version of pandoc other than your default system version can be provisioned via `pandoc::pandoc_activate()`
   - block anchors now reflect the title of the block instead of the generic "callout1"
   - instructor notes summary page displays the title of the instructor notes
   - fixed a test that prevented the binaries from being built on the R universe
   - All features will automatically roll out on Monday evening
 - [{pegboard} fixed a test broken by design](https://github.com/carpentries/pegboard/pull/127)
 - [update workbench documentation](https://github.com/carpentries/sandpaper-docs/pull/142)
   - fix old CONTRIBUTING and LICENSE with modern versions
   - add a makefile with serve and validate because I finally figured out how
     to do that from the command line (thanks to
     https://github.com/carpentries/workbench/issues/50)
 - fixed the failing GitHub actions in our feeds
   [feeds.carpentries.org#77](https://github.com/carpentries/workbench/issues/50)
 - Reviewed PRs for the swc site
 - Transitioned Astronomy Python

#### What did you struggle with?

😶

#### What would you like to work on next week?

 - Organize and triage bugs for The Workbench
 - submit talk for US RSE
 - for the future
   - work on {tinkr} updates to parse in-chunk options
   - work on code handout

#### Where do you need help from Toby?

Please help triage any new issues in The Workbench as best you can before I get
back on Wednesday.

#### What did you learn this week?

🥺

### Date: 2023-05-10

#### Who did you help this fortnight?

It's really hard to keep track of this, but here are some things:

 - helped a bunch of people by posting about [the weirdness with MASS and the new version of R on Mastodon](https://fosstodon.org/@zkamvar/110266431268029158)
 - gave feedback to Maneesha about the difficulty for getting MFA set up for many folks
 - directed Malvika to Toby for a question about Netlify
 - provided our links to a11y advice for Brynn

#### Who helped you this fortnight?

This list is a lot longer, but I cannot compile everything now

 - Alyica (aka The Gif-er, aka The Best) remade the videos that I made for the tweets so that they were more clear. 
 - Alycia, Karen, and Maneesha by providing advice on how to respond to a frustrating comment
 - Toby and Erin for being at my beck and call for random things during the transition


#### What did you achieve?

I have not had time to work on this for over two weeks, so this means that I've
wracked up a whole hell of a lot of contributions on GitHub: If I were to list
out everything I did, it would just be ridiculous. 


 - I have officially transitioned nearly all of our lessons.
   - This consisted of [over 125 commits to the transition workflow](https://github.com/swcarpentry/shell-novice/commits?author=zkamvar&since=2023-04-24&until=2023-05-11)
   - There were many places where I had to create manual pull requests to fix little issues like gaps in the blocks
   - Across our curricula, [60 issues were closed](https://github.com/search?q=user%3Aswcarpentry+user%3Adatacarpentry+user%3ALibraryCarpentry+label%3Apre-workbench&type=pullrequests&ref=advsearch&s=updated&o=desc) (the results say 61, but one of them is an accidental closure of a zenodo release).
   - The workshop "lessons" remain, though these are not technically "lessons"
     because (except LibraryCarpentry), they do not have any episodes. Since all
     the lessons are episode-centric, I want to do something different with these
   - The Astronomy Curriculum was not transitioned because it was not included
     in my list of lessons. This will happen on Monday.
 - released [{sandpaper} 0.11.16](https://github.com/carpentries/sandpaper/releases/tag/0.11.16), which fixes a bug in `serve()`
 - Received 20 issues across sandpaper, workbench, varnish and pegboard
   - https://app.asana.com/0/0/1204463369377016/f 
   - https://app.asana.com/0/0/1204464831962828/f 
   - https://app.asana.com/0/0/1204477229642479/f 
   - https://app.asana.com/0/0/1204477600584214/f 
   - https://app.asana.com/0/0/1204480644417251/f 
   - https://app.asana.com/0/0/1204480694943114/f 
   - https://app.asana.com/0/0/1204498060398312/f 
   - https://app.asana.com/0/0/1204500435662670/f 
   - https://app.asana.com/0/0/1204518317670865/f 
   - https://app.asana.com/0/0/1204519079257164/f 
   - https://app.asana.com/0/0/1204525477475957/f 
   - https://app.asana.com/0/0/1204540748598675/f 
   - https://app.asana.com/0/0/1204540874533124/f 
   - https://app.asana.com/0/0/1204541378265800/f 
   - https://app.asana.com/0/0/1204541562357011/f 
   - https://app.asana.com/0/0/1204553583188327/f 
   - https://app.asana.com/0/0/1204555530052589/f 
   - https://app.asana.com/0/0/1204562303037050/f 
   - https://app.asana.com/0/0/1204566118449970/f 
   - https://app.asana.com/0/0/1204572068372976/f
 - Documented various things in the workflow

#### What did you struggle with?

A lot of things, but I got through them. 

#### What would you like to work on next week?

 - Transition the astronomy lesson
 - Organize and triage bugs for The Workbench
 - draft talk submission for US RSE
 - for the future
   - work on {tinkr} updates to parse in-chunk options
   - work on code handout

#### Where do you need help from Toby?

Just keep doing what you're doing. 

#### What did you learn this fortnight?

No matter how much you communicate or how much dialogue you have with someone,
there is no guarantee that they will be looking at things that matter until it's
too late. 

### Date: 2023-04-21

#### Who did you help this week?

 - Toby by debugging chisel
 - Nathan Porter by fixing an accidentally translated Etherpad

#### Who helped you this week?

 - Toby is the MVP this week for doing things like creating slides for me,
   communicating with maintainers, creating styles PRs, creating lesson
   releases, being there to listen to me whinge
 - Danielle for contacting instructors of upcoming lessons for the next month
   to tell them about the workbench
 - Alycia for taking COPIOUS notes during my community discussions and being
   super understanding when I had to cancel the workbench meeting at the very
   last minute
 - Maneesha and Erin by figuring out a path forward (ha!) for broken paths
   for `code/` in swc lessons 
 - Scott Chamberlain by debugging the ORCiD API that we were using his old,
   deprecated package for. 
 - Eli by opening an issue to get ORCiD integration for AMY.
 - All the maintainers by being patient with me
 - Erin, Vini, and Toby by doing so damn well at updating and leading maintainer
   onboarding
 - Erin for validating that she could build and preview lessons locally
 - Karen and Kelly for addressing the issues remaining in the bonus modules repo
 - Athanasia Mownickel for providing good testimony during the community discussion


#### What did you achieve?

This week was spent on the workbench transition, trying to get things in order,
fixing random stray bugs that made my life easier with the transition and, of
course, performing transitions of five lessons. I'm pretty proud of my
accomplishments this week and I'm ready to do the transitions on Monday. 

 - Transitioned five lessons:
   - stored the archives in google drive (to be uploaded to AWS Glacier once Rob figures it out)
   - https://datacarpentry.org/sql-ecology-lesson/
   - https://librarycarpentry.org/lc-spreadsheets/
   - https://swcarpentry.github.io/python-novice-inflammation/
   - https://librarycarpentry.github.io/lc-git/
   - https://carpentries.github.io/instructor-training-bonus-modules/
 - {pegboard} fixes for link parsing and objectives/questions insertion
   - https://github.com/carpentries/pegboard/pull/121
   - https://github.com/carpentries/pegboard/pull/122
   - https://github.com/carpentries/pegboard/pull/123
   - https://github.com/carpentries/pegboard/pull/124
 - {chisel} fixed ORCiD API change
   - [add a workaround](https://github.com/carpentries/chisel/pull/1)
   - [add a fix](https://github.com/carpentries/chisel/pull/2)
 - Lesson Release Workflow
   - I tested and re-tested the release workflow
   - Updated [Release Documentation](https://github.com/carpentries/lesson-transition/blob/5327f31bc998de37176939bf90e3f1b2170a42b1/release-workflow.md)
   - Updated [Release Testing script](https://github.com/carpentries/lesson-transition/blob/5327f31bc998de37176939bf90e3f1b2170a42b1/run-transition-test.sh)
     with a countdown and instructions
   - Make sure Lessons have [`lang` and `analytics` config items](https://github.com/carpentries/lesson-transition/commit/29dbfd04ea96b17d848d7d89b04c9e902157ab98).
     We do not use these now, but we will in the future.
   - Found really weird and [nasty bug with control characters in markdown](https://github.com/ropensci/tinkr/issues/96)

#### What did you struggle with?

I struggled a bit on Thursday because nothing was going right and I lost time to
transition the lessons I wanted to transition. 

#### What would you like to work on next week

 - just blast through a whole fuckload of lessons in the transition
 - for the future
   - work on {tinkr} updates to parse in-chunk options
   - work on code handout

#### Where do you need help from Toby?

Just keep doing what you're doing. Please make sure the maintainers check the
links in the setup document.

#### What did you learn this week?

It's important to take the time to make sure to do things right rather than
speeding through decisions. 

### Date: 2023-04-14

#### Who did you help this week?

 - Heather Turner, by showing her what [{pegboard} can do for her slide notes](https://fosstodon.org/@HeathrTurnr/110192455478898390)
 - Elio Campitelli by [helping with a {knitr} question](https://mastodon.social/@eliocamp/110188298104737893)
 - Wouter Deconinck by clarifying how we will proceed with styles
 - Maneesha by debugging a frustrating Jekyll thing
 - Matthier Bruneaux by clarifying the jQuery vulnerability warning
 - Rob and Kari by making them owners of the LC and SWC orgs
 - Ben Companjen by answering questions about the workshop template


#### Who helped you this week?

 - Alycia by reviewing my last-minute Dovetail blog post (mostly authored by Toby)
 - Toby by forcing me to sit down and actually plan out what we need to do for
   the transition and agreeing to take on tasks that I didn't have time to do
 - Erin for being super patient, encouraging me to seek help from the team, and
   providing lists of maintainer-less lessons and retired maintainers
 - Every single person who was responsive to pull requests in the Maintainer
   community
 - The Instuctor Training team for being patient with my panicky replies about
   links
 - Joel Nitta by sharing his workbench lesson
 - Scott Chamberlain by explaining how we can make the problemated Jekyll Gem our own
 - Eli by providing links to his GHA workflows for a11y tests


#### What did you achieve?

This week was spent ramping up for The Workbench transition by coallating the
lessons that we need to transition, planning the transition tasks that need to
be done and delegating tasks to Toby. It's been a tough week of trying to make
things work in the lesson transition and make sure that I have everything
organized for the transition.

Here's the breakdown of what happened:

 - [created scripts for all the repositories](https://github.com/carpentries/lesson-transition/commit/a811fb7416e1b243ee0522624c42da8cbf4a6e5f)
 - [created a transition schedule landing page](https://carpentries.github.io/workbench/transition-schedule.html)
   - this lists the repositories to be transitioned and the tracking issue for each repository
   - each repository has one issue (tagged lesson) with a tasklist at the top to monitor things that need to be fixed.
   - [created function to monitor lesson
     issues](https://github.com/carpentries/lesson-transition/commit/d970f5a8d8504458a63d44ce2ba069b8759c689c).
     This allows me to find patterns while I'm iterating to determine if I need
     to add a function to the transition workflow or to a given lesson
   - [Blogged about my tasklist function](https://zkamvar.netlify.app/blog/gh-task-lists/)
 - Ran an initial transition on all of the lessons and created pull requests where there were structural issues
 - Added [transition workflow
   document](https://github.com/carpentries/lesson-transition/blob/main/transition-workflow.md)
   describing the iteration workflow for determining how problems arise in the
   lesson
 - opened a whole bunch of pull requests in a whole bunch of repositories. 
 - created previews for the lessons that want to transition early:
   - https://github.com/fishtree-attempt/r-novice-gapminder-es
   - https://github.com/fishtree-attempt/lc-marcedit
   - https://github.com/fishtree-attempt/lc-data-intro-archives
   - https://github.com/fishtree-attempt/sql-ecology-lesson
   - https://github.com/fishtree-attempt/matlab-novice-inflammation
   - https://github.com/fishtree-attempt/python-novice-inflammation
   - https://github.com/fishtree-attempt/image-processing
   - https://github.com/fishtree-attempt/lc-wikidata
   - https://github.com/fishtree-attempt/openrefine-socialsci
   - https://github.com/fishtree-attempt/instructor-training-bonus-modules
   - https://github.com/fishtree-attempt/lc-sql


I am le tired.

#### What did you struggle with?

*gestures around wildly*

#### What would you like to work on next week

 - just blast through a whole fuckload of lessons in the transition
 - release the instructor training bonus module lesson
 - survive the community call (I haven't prepared anything `-_-`)
 - continue to organise transition script to make sure all of our lessons work
 - for the future
   - work on {tinkr} updates to parse in-chunk options
   - work on code handout

#### Where do you need help from Toby?

Let me know if you need help with lesson release and please provide me with the
sign up spreadsheet for the transition times.

#### What did you learn this week?

I can't even

### Date: 2023-04-07

#### Who did you help this week?

 - (attempt) Maneesha with her Jekyll woes, but I couldn't
 - (attempt) Infrastructure team by clarifying how we use our URLs
 - Karen and Kelly by taking notes in the Trainer meeting
 - (attempt) Karen by clarifying the link kerfuffle
 - Workbench Beta team members by cancelling the meeting I had not prepared for
 - Eli by providing context for a _really old_ JS library in our website
 - Maneesha by clarifying about the fact that the Curriculum Team has not met
   in a while and that the next meeting may not be the best time for her to
   hop in.

#### Who helped you this week?

 - Toby by providing a good conversation about management
 - Toby by offering help with things I need to do with the workbench release
 - Talisha by switching lab meeting times with me
 - Kelly by confirming that she still has maintainer rights after I moved her
   to the team
 - Erin by listening to my panicky-ass ramblings about needing lists of
   maintainers and then sending me spreadsheets of maintainers

#### What did you achieve?

Much of this week was spent attempting to improve the lesson transition process
so that it can be workable in a more secure manner and so it does not blow up 
the size of your local clone. I also had that little thing about the workbench
beta phase coming to an end, which was a bit anticlimactic. I mean, Kari
congratulated me and my first reaction was "wait, why am I being congratulated?"
Tuesday was particularly nerve-wracking because there was confusion about what
was going to happen with our URLs in the instructor training repository and I
needed to throw together a 404 page solution PDQ. 

Here's the breakdown:

 - I released our four lessons from beta to the not beta.
 - I sent a message to the r-novice-inflammation lesson offering help (no response)
 - [{sandpaper} added 404 page](https://github.com/carpentries/sandpaper/pull/429)
   - [fixed 404 page that was ugly af](https://github.com/carpentries/sandpaper/pull/431)
 - [{sandpaper} fixed template language and URLs](https://github.com/carpentries/sandpaper/pull/431)
   - [updated R Markdown template repo](https://github.com/carpentries/workbench-template-md/pull/25)
   - [updated R Markdown template repo](https://github.com/carpentries/workbench-template-rmd/pull/39)
 - [(carpentries.org) add landing pages for the instructor training confirmation and events pages](https://github.com/carpentries/carpentries.org/pull/1607)
   - this came from a conversation with Talisha, Kelly, and Karen about what will happen to these pages.
   - the solution was to update the links to point to these pages because Talisha had plans for them to live there in the future.
 - [{pegboard} do not include readme in checks](https://github.com/carpentries/pegboard/pull/117)
 - [{varnish} attempted to fix display bug for definition lists](https://github.com/carpentries/varnish/pull/78)
   - unfortunately [they don't friggen work](https://fishtree-attempt.github.io/python-novice-inflammation/reference.html#glossary-1) :weary:
 - [{renv} addressed an issue with BioConductor lessons for renv 0.17.2](https://github.com/carpentries-incubator/bioc-rnaseq/pull/29#issuecomment-1494615282)
 - I added five zapier workflows to bring in new issues to the workbench components to the workbench roadmap in asana. They kinda work. 

And a special section dedicated to the lesson transition:

 - [enforce token usage for release process](https://github.com/carpentries/lesson-transition/pull/31)
   - Documented [fine-grained PAT usage](https://github.com/carpentries/lesson-transition/blob/main/release-workflow.md#fine-grained-pat-preferred)
   - Documented [adding tokens to vault](https://github.com/carpentries/lesson-transition/blob/main/release-workflow.md#adding-tokens-to-your-environment)
   - Documented [testing release process](https://github.com/carpentries/lesson-transition/blob/main/test-workflow.md)
 - Added [function to auto-close open PRs](https://github.com/carpentries/lesson-transition/commit/254f9ccf517cb056325a8ab33a69e186b471599e) (this was a PITA to get set up)
   - created [comment template language for closed prs](https://github.com/carpentries/lesson-transition/blob/main/close-pr-msg.md) (note: I updated it to appeal to humanity)
 - Created and ran [function to create workbench maintainer teams](https://github.com/carpentries/lesson-transition/commit/3fdba9d15a8dd5fda69fb4702cb67e519b8feb91)
   - reasoning: we do not want maintainers accidentally pushing to the
     repository, so we change their current team to read only. As they confirm
     that they want write access, then we can move them over to the new team,
     which has maintain access. Once the teams have the same number of people,
     we can delete the workbench team. Case in point, the [instructor training
     access](https://github.com/carpentries/instructor-training/settings/access)
     has three members of the team that have not confirmed access.
 - added the carpentries bot to all of the lessonr respositories
 - added functions to be used during transition
   - added function to [add a workflow token to a repository](https://github.com/carpentries/lesson-transition/commit/e0edc39bf20dc593e75371d852a8a19d99c24869)
   - added function to [set team to read](https://github.com/carpentries/lesson-transition/commit/74038822b6bb378fb60096defc4d95852cd79ae4) 
 - [transformed datacarpentry/organisation-geospatial](https://github.com/carpentries/lesson-transition/issues/26)
 - [transformed datacarpentry/r-intro-geospatial](https://github.com/carpentries/lesson-transition/issues/25) (still need to push to github and notify maintainers)

#### What did you struggle with?

I am still behind in a lot of things and I have a strong suspicion that I never
actually communicated with the lesson maintainers that they will need to work on
closing their open pull requests this month. If this is true, then we have a lot
of work ahead of us as there are > 100 PRs open in the top four repos alone.

I wasn't able to get the dovetail blog post written and I wasn't able to plan
for the workbench beta phase meeting that was supposed to happen on Tuesday.

I'm struggling a lot with the fact that I still have to think about getting
things organized for lesson release, communicating with maintainers about 
expectations, finding a method to organize and track issues that we create about
the lesson transition, and dealing with fallout from maintainers who will be
caught in their unawares about the PR debacle. 

The link issue that Karen brought up is a real issue and I just really had no
time to plan for how to handle the fact that a lot of our links are going to 
break becuase we have never had any good plans for redirects.

I have so many damn red items in Asana and a lot of them are communications related.

#### What would you like to work on next week

 - just blast through a whole fuckload of lessons in the transition
 - reach out to r ecoloy and librarycarpentry maintainers (from seven weeks ago)
 - reach out to maintainers of PR-burdened lessons and ???
 - continue to organise transition script to make sure all of our lessons work
 - for the future
   - work on {tinkr} updates to parse in-chunk options
   - work on code handout

#### Where do you need help from Toby?

Literally just craft a message to the maintainers letting them know that they 
have until May to address the PRs and to contact the curriculum team if they
need help. We really really really really really should not delay on this and I
have already delayed longer than it needs to be. 

I think a good strategy is to:

1. create a simple message to send to the list and send it. I don't care what it says, just send it.
2. craft a message for github issues and add it to the lesson transition repository. I will create a script that can post it on the repositories.

I will work on the script to send that on Monday, tagging everyone who has write access to the repository.

#### What did you learn this week?

I found out there is a function called `rle()` that will count runs of values.
If I had known about it when processing the lc-r lesson, I wouldn't have had
to [reverse-engineer it with table and cumsum](https://github.com/carpentries/lesson-transition/blob/74038822b6bb378fb60096defc4d95852cd79ae4/librarycarpentry/lc-r.R#L40-L46)

### Date: 2023-03-31

#### Who did you help this week?

 - Erin by agreeing to cancelling our Curriculum Team meeting when we
   both had oatmeal brains
 - Talisha, Kelly, and Karen by clarifying and strategising where the non-lesson
   confirmation page should go in our infrastructure (on the main site, where
   Talisha has already built a page for it on the beta site).

#### Who helped you this week?

 - Kelly by testing out the installation of The Workbench on her
   system and giving me a video recording showing me some missing connections in
   her concept map for RStudio.
 - Alycia provided guidance for how to request a new blog post
 - Murray opened an issue for his request
 - Vini shared with me the github skillup lesson for maintainers
 - Trevor Keller opened a PR to lint the workbench template, which allowed me
   to realize that I need to get on fixing that.

#### What did you achieve?

This week was heavily focussed on the Lesson Transition workflow and gathering
information about lessons that need to be transitioned. I had documented the
workflow, updated the packages that go with the workflow, and made patches to
lessons. It's been a fairly exhausting week. 

Here's a breakdown of what happened:

 - (lesson-transition) Update Documentation 
   - see <https://github.com/carpentries/lesson-transition#transitioning-carpentries-lessons>
   - This includes how to clone, how to setup, what the storage requirements are, and mermaid diagrams for the process.
 - (lesson-transition) Use the [{pandoc}](https://cderv.github.io/pandoc/) R
   package to [provision a consistent verison of
   pandoc](https://github.com/carpentries/lesson-transition/commit/52f88ab5223822773f7de35e315079d8a013a1b1)
   for the transition.
 - (lesson-transition) add list of lessons to be transitioned in an issue: <https://github.com/carpentries/lesson-transition/issues/23>
 - (lesson-transition) open issue to track issues in python-novice-inflammation <https://github.com/carpentries/lesson-transition/issues/22>
   - [{pegboard} opened weird alt text issue with mixed quote
     marks](https://github.com/carpentries/pegboard/issues/112). Ultimately:
     this was one I fixed with search and replace instead of preserving the
     puncutation.
   - [(python-novice-inflammation) fix bad syntax in
     setup](https://github.com/swcarpentry/python-novice-inflammation/pull/1031).
     NOTE: the reason this was like this in the first place was due to an
     overzealous ideal of limiting the line length combined with the liquid
     syntax, which is not portable markdown. 
 - (lesson-transition) open issue to track issues in r-novice-inflammation (currently broken)
   - Fixed AMY data discrepancy for the maintainer of the r-novice-inflammation.
     Amy had no record for that lesson, but the maintainer was part of the team.
 - Re-run stats on the [number of open pull requests](https://docs.google.com/spreadsheets/d/1Cc3i_XQTS4nQ1rjkG0Exb5Oe0TVmQCU2HdpL4VJYsPE/edit#gid=1259841966)
    - python ecology lesson and r-novice inflammation are in the lead with PRs in the high 20s
 - [{tinkr} release version 0.2.0 to CRAN](https://github.com/ropensci/tinkr/releases/tag/0.2.0)
 - {pegboard} made updates that will help my translation process by highlighting problems in external files
   - [0.5.0 update validator to include ALL files](https://github.com/carpentries/pegboard/releases/tag/0.5.0)
     - [(instructor-training) opened PR to fix http links](https://github.com/carpentries/instructor-training/pull/1519)
   - [0.5.1 update div support](https://github.com/carpentries/pegboard/releases/tag/0.5.1)
 - [(instructor-training) add RStudio file](https://github.com/carpentries/instructor-training/pull/1518)
 - [(workbench-template-md) reviewed a PR that linted the markdown and yaml files](https://github.com/carpentries/workbench-template-md/pull/24)

#### What did you struggle with?

The reading and reflection day was more of rstress and ranxiety day for me.
I was attempting to update the documentation for the Lesson Transition and then
move on to adding tweets for The Workbench when I ran into a whole bunch of
negative feelings about the announcement and I struggled with the feeling that
whatever I would say would not be true because yes, while The Workbench is
easier to use than styles, it's a pretty low bar. 

Ultimately, I recognise that this is an improvement and I should tout it as such
and I'm trying to get better, but it's just really difficult. I think there's a
lot of stress right now because I am near the launch of this and we have no
capacity as a team to give the support we need to give to get the maintainers
past the finish line of resolving the old PRs. I feel like the Curriculum Team
is also floundering a bit due to everyone having too much on our plates plus
various life changes happening all in one quarter. I feel guilty asking for help
because I know that everyone is struggling in some way or another. 

#### What would you like to work on next week

 - reach out to r ecoloy and librarycarpentry maintainers (from six weeks ago)
 - reach out to maintainers of PR-burdened lessons and ???
 - continue to organise transition script to make sure all of our lessons work
 - for the future
   - work on {tinkr} updates to parse in-chunk options
   - work on code handout

#### Where do you need help from Toby?

Did you and Vini reach out to any lessons other than python-novice-inflammation?

#### What did you learn this week?

Not sure. I've been going pretty full on. 

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
