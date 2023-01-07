# Meeting Notes

## Table of Contents

 - [2023-01-06](#date-2023-01-06)

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
