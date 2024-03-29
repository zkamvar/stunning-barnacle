# Meeting Notes

## Table of Contents

 - [2021-12-17](#date-2021-12-17)
 - [2021-12-10](#date-2021-12-10)
 - [2021-12-03](#date-2021-12-03)
 - [2021-11-19](#date-2021-11-19)
 - [2021-11-12](#date-2021-11-12)
 - [2021-11-05](#date-2021-11-05)
 - [2021-10-29](#date-2021-10-29)
 - [2021-10-22](#date-2021-10-22)
 - [2021-10-15](#date-2021-10-15)
 - [2021-10-01](#date-2021-10-01)
 - [2021-09-24](#date-2021-09-24)
 - [2021-09-17](#date-2021-09-17)
 - [2021-09-10](#date-2021-09-10)
 - [2021-08-27](#date-2021-08-27)
 - [2021-08-20](#date-2021-08-20)
 - [2021-08-13](#date-2021-08-13)
 - [2021-07-30](#date-2021-07-30)
 - [2021-07-23](#date-2021-07-23)
 - [2021-06-04](#date-2021-06-04)
 - [2021-05-28](#date-2021-05-28)
 - [2021-05-21](#date-2021-05-21)
 - [2021-05-14](#date-2021-05-14)
 - [2021-05-07](#date-2021-05-07)
 - [2021-04-30](#date-2021-04-30)
 - [2021-04-23](#date-2021-04-23)
 - [2021-04-16](#date-2021-04-16)
 - [2021-03-31](#date-2021-03-31)
 - [2021-03-23](#date-2021-03-23)
 - [2021-02-23](#date-2021-02-23)
 - [2021-02-16](#date-2021-02-16)
 - [2021-02-09](#date-2021-02-09)
 - [2021-02-02](#date-2021-02-02)
 - [2021-01-26](#date-2021-01-26)
 - [2021-01-19](#date-2021-01-19)
 - [2021-01-11](#date-2021-01-11)
 - [2021-01-05](#date-2021-01-05)

### Date: 2021-12-17

#### Who did you help this week?

 - [I helped Michael get set up with a new {sandpaper} lesson.](https://github.com/MCMaurer/Rewrite-R-ecology-lesson/pull/1)
 - I helped Karen and Omar by suggesting Vimeo as an alternative platform for our teaching videos.
 - I helped Dan by running the maintainer meetings

#### Who helped you this week?

 - Michael helped me by trying out the lesson infrastructure and letting me know about the surprises that he found with the cache.
 - Kate, Jonah, Naupaka, and Françios helped me by reviewing the blog post and clarifying their consent to be named.
 - François helped me by reminding me that it was okay to take time off. 
 - Erin helped me by showing me how to schedule a blog post and reminding me to check in with my therapist (indirectly)

#### What did you achieve?

 - [(LIC) I opened the blog post about the Lesson Infrastructure Commitee](https://github.com/carpentries/carpentries.org/pull/1264)
 - I identified issues on iOS for the new lesson frontend
 - [{actions} I found a bug in {pak}](https://github.com/r-lib/pkgdepends/issues/267)
 - [{actions} I am starting to test out placing renv functions in a formal package](https://github.com/carpentries/actions/pull/34)
 - [{actions} I created the {vise} package that wraps {renv}](https://github.com/zkamvar/vise)
 - [{sandpaper} I added the `serve()` function](https://github.com/carpentries/sandpaper/pull/220)
 - [{sandpaper} I added minor support for the instructor block](https://github.com/carpentries/sandpaper/pull/219)
 - [{pkgdown} I created a PR that addresses code overflow](https://github.com/r-lib/pkgdown/pull/1969)

#### What did you struggle with?

I struggled with focus a bit. I had to take some time off on Tuesday and 
yesterday because I felt a lot like a block of tofu. I have decided to take some
extra days on my vacation so that I can truly decompress before I get back to it.

#### What would you like to work on next week?

* nothing, I'm going to be on vacation

When I come back:

* set up instructor page
* clean up github actions further
* port sandpaper's {renv} functions to {vise}

#### Where do you need help from François?

* Nowhere

#### Any other topics

All in all, it's been a good year and I am looking forward to 2022!

### Date: 2021-12-10

(completed on 2021-12-13)

#### Who did you help this week?

- I helped Karen fix formatting in a blog post
- I helped Maxim and Sarah understand how [a new gem introduced into github pages
  was introducing an unexpected feature that had unintended consequences](https://github.com/carpentries/styles/issues/633#issuecomment-990533187)
- I helped Alycia by pointing to evidence that our template licensing does not affect the licensing of the lesson contents.
- I helped Alycia by pointing to resources that provide the reasons why to move from master to main for the default git branch.

#### Who helped you this week?

- Alycia helped me by reiviewing the LIC blog post. 
- François helped me by confirming that the 502 error from the etherpad at 02:00
  UTC was due to a backup process occurring.
- Toby helped me by explaining the scope of the metadata talks
- The rladies account helped me understand why the r-raster-geospatial lesson was giving errors [r-raster-vector-geospatial#363](https://github.com/datacarpentry/r-raster-vector-geospatial/issues/363)

#### What did you achieve?

 - I completed the GDPR training
 - I had my performance review meeting
 - I drafted the first draft of the blog post for the lesson infrastructure committee project
 - [{pegboard} fixed an old minor issue that would insert redundant headings on lesson conversion](https://github.com/carpentries/pegboard/pull/71)
 - [(lesson-transition) figure out how to update submodules](https://github.com/data-lessons/lesson-transition/commits?author=zkamvar&since=2021-12-06&until=2021-12-12)
 - [(sandpaper-docs) updated the ubuntu setup instructions](https://github.com/carpentries/sandpaper-docs/commit/55315641242f64e59ae0e9d440a9615c32e42e34)
 - [started a rudimentary test of python via reticulate](https://github.com/zkamvar/expeditious-screamer/commit/83af6a8033701f42033921aef6723bd064643cc5)
 - [{tinkr}/{knitr} opened a PR that would allow us to parse yaml chunk options in {tinkr}](https://github.com/yihui/knitr/pull/2083)

#### What did you struggle with?

I again struggled with confidence. I had agonised over the wording of my blog 
post in relation to the volunteers who spoke with me about their experiences. I
was worried that they would read the blog post and think that I did not 
incorporate their viewpoints in there. 

#### What would you like to work on next week?

* Documentation
* setting up the infrastructure to split the instructor page
* using centralised github workflows

#### Where do you need help from François?

* Not sure

#### Any other topics

I think one thing I need to work on is to understand where and when I need help
from my supervisor.

### Date: 2021-12-03

(completed on 2021-12-06)

#### Who did you help this week?

- No one

#### Who helped you this week?

- Alycia helped me by reiviewing the LIC documents.

#### What did you achieve?

 - I updated the documentation website for sandpaper by splitting the landscape
   document into parts
 - I browsed and tested the pkgdown updates to ensure it did not break sandpaper
 - I solicited feedback from Alycia WRT the LIC
 - I started to brainstorm a roadmap for the lesson infrastructure with François
 - I solicited further times to meet with the metadata group

#### What did you struggle with?

I struggled with my mental health. Things have been very tough these past five
weeks.

#### What would you like to work on next week?

* Documentation
* Draft blog post for Q3 project

#### Where do you need help from François?

* Not sure

#### Any other topics

I had a short week this week where I suffered from a lot of anxiety and ended
up taking sick time on Friday, so the list of accomplishments is small. Part of
this has been due to the time change and part has been due to things I'm dealing
with in my personal life. I just had a vacation, but it did not feel like one.
I'm hoping that the end of the year will be better. Part of my coaching is for 
me to add a self-affirmation every day and I can not say that I have been 
successful at it, but I will try, which will hopefully get me out of this funk.

### Date: 2021-11-19

#### Who did you help this week?

- I don't think I helped anyone this week, TBH

#### Who helped you this week?

- Once again, the entire team has been really helpful in helping me deal with 
  all sortsa stress.

#### What did you achieve?

I did a whole bunch of things that centered around [updating the github actions
to use ubuntu runners instead of macos](https://github.com/carpentries/sandpaper/pull/211) along with news from renv.

I [created a plan for the learner/instructor view structure in varnish](https://github.com/carpentries/varnish/issues/12). 

I sent an email to plan a meeting with the Zenodo folks, but I was too late :disappointed:

#### What did you struggle with?

I struggled with my mental health. Things have been very tough these past three
weekss.

#### What would you like to work on next week?

* Documentation

#### Where do you need help from François?

* At the moment, nothing

#### Any other topics

I am le tired.

### Date: 2021-11-12

#### Who did you help this week?

- I helped a community member understand the terms of the license for the lesson
  "template"

#### Who helped you this week?

- François and Omar helped me understand why I missed a comment on our Disqus about the new infrastructure
- The entire core team has been really supportive while I've been going through a difficult time

#### What did you achieve?

This week was still a bit of a mess, but lesso of a mess than last week. I was actually able to get things done!

* [(lesson transition) I posted the transitioned lessons to GitHub](https://github.com/fishtree-attempt)
* [(styles) I opened a PR to address a styling issue](https://github.com/carpentries/styles/pull/631)
* [{sandpaper} I fixed a deployment bug and errors that were coming from the new {glue}](https://github.com/carpentries/sandpaper/pull/207)
* I sent out the reminder email for the LIC revival interviews
* I interviewed Maxim about his experiences
* I completed the self and peer review
* I spoke with the frontend contractor about the results and inspected them for changes that we wish to make.

#### What did you struggle with?

I struggled with my mental health. Things have been very tough these past two
weekss.

#### What would you like to work on next week?

* Plan meeting with Zenodo folks WRT lesson metadata
* Outline plan to incorporate Frontend scripts into the new infrastructure.

#### Where do you need help from François?

* At the moment, nothing

#### Any other topics

I am le tired.

### Date: 2021-11-05

#### Who did you help this week?

- I helped Erin figure out the error that was happening with the Zenodo publication process for the instructor training lesson.

#### Who helped you this week?

- François, Karen, and Kari helped me by strategising which workshop to attend during CZI
- Naupaka helped me by giving me a new perspective of the LIC for my report

#### What did you achieve?

Hoo boy this week was a mess because I should remember that if I'm attending a
conference, even if it is virtual, it will take ALL of my time. I also had to
take half a sick day for personal reasons. Much of what I did was work in the 
lesson transition script

* [{pegboard} remove root and layout yaml items for sandpaper](https://github.com/carpentries/pegboard/pull/69)
* Interviewed Naupaka
* Attended CZI
* [(lesson transition) I updated the script for the lesson transition to use git-filter-repo to preserve commits](https://github.com/data-lessons/lesson-transition/pull/4)
* [(lesson transition) I added a script to create a new repository and add the bots team to it](https://github.com/data-lessons/lesson-transition/commit/028131926bcf8de665ebee911cadd1a38279b1c6)

#### What did you struggle with?

* conferences

#### What would you like to work on next week?

* Complete self and peer review of team mates
* Sift through output of frontend contractor and come up with plan to implement
* Post the transitioned lessons to GitHub
* Plan meeting with Zenodo folks WRT lesson metadata

#### Where do you need help from François?

* At the moment, nothing

#### Any other topics

APIs are scary things. 

### Date: 2021-10-29

#### Who did you help this week?

- I helped myself and Alycia find where the self and peer evaluations were (by
  bugging the help desk slack channel)

#### Who helped you this week?

- Erin helped me by hopping on a call with DNAnexus
- Erin and Maneesha helped me by pointing to the location of the peer evaluations
- John MacFarlane (pandoc) helped me by quickly finding the cause of and fixing 
  [a bug that popped up in pandoc 2.15](https://github.com/jgm/pandoc/issues/7639).

#### What did you achieve?

I feel like I did not get that much done this week. This is partially due to the
fact that I had vacation in the middle of the week, but I think it's also 
because I did have interviews that I was doing in the week, so those took some
time.

* [{pegboard} process inline image attributes](https://github.com/carpentries/pegboard/pull/67)
* [{sandpaper} add function `set_dropdown()`](https://github.com/carpentries/sandpaper/pull/203)
* [{sandpaper} fix package discovery](https://github.com/carpentries/sandpaper/pull/200)
* [found bug in pandoc](https://github.com/jgm/pandoc/issues/7639)
* Sent out interview requests from the former LIC members
* Interviewed three former members thus far
* Completed most of self-review and ~1/4 peer review

#### What did you struggle with?

* performance review stuff is always hard.

#### What would you like to work on next week?

* Complete transition plan to use git-filter-repo to include only commits for
  the content of the lesson. 
* Post the transitioned lessons to GitHub
* Plan meeting with Zenodo folks WRT lesson metadata

#### Where do you need help from François?

* At the moment, nothing

#### Any other topics

I'm glad that one of my interviewees pointed out that the git history in the
lessons is used by instructors as an example of how you can trace back the 
history of something and see exactly how you made an impact on a project. This
reminded me to look up git-filter-repo and realise that it was exactly the tool
I needed to include the old commits. The only challenge I have right now is to 
rewrite the script to transform the lesson on top of the existing lesson.

### Date: 2021-10-22

#### Who did you help this week?

- I helped maintainers in my testing for the transformation script by fixing
  small bugs in their repositories:
  - https://github.com/datacarpentry/astronomy-python/pull/91
  - https://github.com/carpentries-incubator/python-packaging-publishing/pull/89
  - https://github.com/carpentries-incubator/jekyll-pages-novice/pull/266
  - https://github.com/carpentries-incubator/SDC-BIDS-dMRI/pull/192
- I [helped Omar with a bug in MailChimp](https://zkamvar.github.io/fix-mailchimp)

#### Who helped you this week?

Alycia, François, and Michael helped me proofread an email I will send out to
former members of the lesson infrastructure committee next week.

#### What did you achieve?

Much of my work this week was the same as last week: spent on translations and
addressing things that popped up in {pegboard} and {tinkr} based on what I
found. 

* [{tinkr} yet another math parsing issue fixed](https://github.com/ropensci/tinkr/pull/60)
* [{pegboard} fix dang liquid tags](https://carpentries.github.io/pegboard/news/index.html#pegboard-0-0-0-9030)
* [{sandpaper} (0.0.0.9060--9063) fix issues with yaml, lesson title, and package cache](https://carpentries.github.io/sandpaper/news/index.html#sandpaper-0-0-0-9063)
* [(carpentries.org) add note that the LIC is on hiatus](https://github.com/carpentries/carpentries.org/pull/1207)
* [(lesson transition) tested transition with all the repositories from the alpha testing](https://github.com/data-lessons/lesson-transition/commits?author=zkamvar&since=2021-10-18&until=2021-10-23)
* Wrote protocol for cycling tokens in The Carpentries Apprentice in the systems wiki
* Created draft for the LIC revival listening session email
* Organised historical document for the LIC revival
* Understood that the GitHub workflows _will_ show up when they are needed.

#### What did you struggle with?

* kramdown. ugh. 

#### What would you like to work on next week?

* Email former LIC members
* Post the transitioned lessons to GitHub
* Plan meeting with Zenodo folks WRT lesson metadata

#### Where do you need help from François?

* At the moment, nothing

#### Any other topics

None :)

### Date: 2021-10-15

#### Who did you help this week?

I provided a response and context to an inquiry that Alycia got about folks
looking for development of a lesson. I also provided reassurance to some
trainers that the problems they were experiencing on their lesson with malformed
links breaking the site would not be a problem with the new infrastructure.

#### Who helped you this week?

Erin is going to bring the vision benefit issue up with CI; Omar reached out to
talk about hex sticker designs. 

#### What did you achieve?

Much of my work this week was spent on translations and addressing things that
popped up in {pegboard} and {tinkr} based on what I found. 

* [(translations) I have set up a general translation script for our lessons](https://github.com/data-lessons/lesson-transition#readme)
* [(translations) Created R for Reproducible Science](https://data-lessons.github.io/r-novice-gapminder/)
* [(translations) Created Incubator Lesson Translation](https://data-lessons.github.io/simple-linear-regression-public-health/)
* [(translations) Migrated R Ecology Lesson to data-lessons](https://data-lessons.github.io/R-ecology-lesson/)
* [{renv} identified caching issue](https://github.com/zkamvar/test-with-renv/pull/17)
* [{sandpaper} added information about renv vis a vie r-universe](https://github.com/carpentries/sandpaper/issues/163#issuecomment-940296757)
* [{pegboard} update liquid tag link parsers](https://github.com/carpentries/pegboard/pull/61)
* [{pegboard} auto-detect lessons with R Markdown vs just markdown (no manual switch needed)](https://github.com/carpentries/pegboard/pull/62)
* [{tinkr} discovered and fixed problem in math parsing](https://github.com/ropensci/tinkr/pull/57)


#### What did you struggle with?

* cache invalidation

#### What would you like to work on next week?

* Investigate why not all of the GitHub Actions show up on new repos
* Document updating the sandpaper workflow tokens
* Plan meeting with Zenodo folks WRT lesson metadata

#### Where do you need help from François?

* At the moment, nothing

#### Any other topics

The vacation was good and very needed

### Date: 2021-10-01

#### Who did you help this week?

I don't know that I actually helped anyone this week :/

#### Who helped you this week?

I am not sure I helped anyone, either :/

#### What did you achieve?

* [{actions} add setup actions for sandpaper and renv](https://github.com/carpentries/actions/pull/28)
* [{actions} add updater for renv](https://github.com/carpentries/actions/pull/30)
* [{pegboard} add documentation for validators](https://carpentries.github.io/pegboard/articles/articles/validation.html)
* [{sandpaper} add landscape article to sandpaper docs (still needs revamping)](https://carpentries.github.io/sandpaper/articles/articles/landscape.html)
* [{sandpaper} update the cache updater workflow to use actions](https://github.com/carpentries/sandpaper/pull/186)
* [{sandpaper} fix bug in monthly workflow where it would run weekly](https://github.com/carpentries/sandpaper/pull/187)
* began testing of r-raster-vector-geospatial... but there were errors in the execution that I did not have time to debug :/

#### What did you struggle with?

* Perhaps the realization that I will have to refactor the infrastructure to use
  ubuntu to build the lessons because there is more support for installing the
  software needed.

#### What would you like to work on next week?

(N.B. this is in two weeks)

* Plan meeting with Zenodo folks WRT lesson metadata
* Test conversion of incubator lessons

#### Where do you need help from François?

* At the moment, nothing

#### Any other topics

Vacation next week; I am unsurprisingly tired.

### Date: 2021-09-24

#### Who did you help this week?

I helped Elizabeth McAulay close an irrelevant issue on the lc-git repository 
that arose when she was fixing the authentication debacle.

I added Kari to the Core team curriculum channel so she could get feeback about
the genomics lesson.

#### Who helped you this week?

* François helped me during our one-on-one with understanding the scope of the project.

#### What did you achieve?

* [{actions} updated the pull request checker action](https://github.com/carpentries/actions/pull/26)
* [{pegboard} massively rewrote the validator methods for](https://github.com/carpentries/pegboard/pull/51)
* [{pegboard} created a handout method in pegboard](https://github.com/carpentries/pegboard/pull/55)
* [{sandpaper} update pkgdown documentation](https://carpentries.github.io/sandpaper/reference/index.html)
* [{sandpaper} update CI to fail early on invalid PRs](https://carpentries.github.io/sandpaper/news/index.html#sandpaper-0-0-0-9052)
* [{sandpaper} began PR to add handout functionality in lessons](https://github.com/carpentries/sandpaper/pull/175)
* [docs: added PR section with images](https://github.com/carpentries/sandpaper-docs/pull/61)

#### What did you struggle with?

* Nothing really, this was a good week.

#### What would you like to work on next week?

* Plan meeting with Zenodo folks WRT lesson metadata
* Move technical documentation into sandpaper
* Test conversion of some incubator lessons

#### Where do you need help from François?

* At the moment, nothing

#### Any other topics

I have vacation in a week, so that will be nice :)

### Date: 2021-09-17

(written on 2021-09-20)

#### Who did you help this week?

I have posted responses to community members inquiring about the future of the
lesson infrastructure WRT Jekyll and the HPC lessons.

#### Who helped you this week?

* Erin really helped me by speaking with me on Thursday evening about the
  planning phase for the Q4 project. She was able to help me understand the
  scope of the project and a bit of the history of the community.
* Alycia, Erin, and François helped reassure me that my fears and axieties
  around my work are relatively normal.

#### What did you achieve?

* Merged branch to integrate {renv} with sandpaper:
  https://github.com/carpentries/sandpaper/pull/158
* Created a sandpaper version of dc-r-ecology https://zkamvar.github.io/dc-r-ecology/
* Revamped and submitted proposal for LIC (changed from communication plan to 
  further research history and find facts surrounding appropriate structure).
* Revamped processing in pegboard to [allow shortcut for sandpaper
  lessons](https://github.com/carpentries/pegboard/pull/50) (because pegboard
  was originally designed to explore the infrastructure, much of the code dealt
  with handling kramdown syntax and assumed as such by default. This fix added
  workrounds for those defaults in a not-so-elegant manner, but one that will
  work in the end).
* [Fixed bug in {tinkr} where numeric parameters would be converted to
  characters, causing downstream {knitr}
  errors](https://github.com/ropensci/tinkr/pull/54). This was in response to
  discovering these [knitr errors in a transation of 
  r-novice-gapminder](https://github.com/zkamvar/r-novice-gapminder/commit/c9b466616d4a46e4a8c7b94d4aa6c7de23bf88ad).
* I started on [an XSL solution to generate a cheat sheet](https://github.com/carpentries/pegboard/commit/1becbdd06ad748d68d78637d8072868e0b081e83),
  but so far it doesn't work that well.

#### What did you struggle with?

* My own brain 🧠.

#### What would you like to work on next week?

* Plan meeting with Zenodo folks WRT lesson metadata
* Move technical documentation into sandpaper
* Document pull request updates on the docs site
* Test conversion of some incubator lessons

#### Where do you need help from François?

* At the moment, nothing

#### Any other topics

Becoming more visible here is definitely going to be a struggle for me to get
used to.

### Date: 2021-09-10

(written on 2021-09-13)

#### Who did you help this week?

I helped Annajiat with an ambiguous error in glosario, other than that, my help
has either been missing or not recorded in the past two weeks. Oh, I helped Kari
by hopping on a call when she needed to rest.

#### Who helped you this week?

* JJ and Christophe helped me get a sense of where quarto was going and how we
  might be able to use it in the lesson in https://github.com/carpentries/sandpaper/issues/161

#### What did you achieve?

* Continued to work on {renv} integration with {sandpaper}
  https://github.com/carpentries/sandpaper/pull/158
   - add workflow and function to update renv cache, with a nice reporter:
     https://github.com/zkamvar/test-with-renv/pull/9
   - revamped continuous integration to run coverage in parallel
   - added a lot of tests for {renv}
   - Generatlly a lot of frstrating tweaking.
* progress on lesson infrastructure committee
  - I was able to make a _little_ progress on the LIC proposal. It's just difficult.

#### What did you struggle with?

* Cache invalidaton
* Continuous integration
* GitHub variables

#### What would you like to work on next week?

* finish quarterly project plan for recruitment of the lesson infrastructure committee.
* merge {renv} pull request

#### Where do you need help from François?

This is still relevant from last time: 

> As both Toby and I are dabbling in bots, I think it would be a good idea to
> coördinate with Maneesha about creating an official carpentries bot account
> similar to https://github.com/ropensci-bot
> 
> Things to consider for the bot account:
>  - How do we control access with 2fa? 
>  - Do we give it broad access for our organizations or do we make it repo-specific?
>  - How often should we recycle tokens and who should be responsible?

#### Any other topics

The pull request for package caching is getting a bit out of hand and I think I 
just need to merge it and deal with any of the repercussions later.

### Date: 2021-08-27

(written on 2021-08-30)

#### Who did you help this week?

I helped Sarah Stevens by adding the update styles workflow to two of her 
incubator lessons. I also approved and merged Erin's addtion to the Handbook for
the CAC consultation rubric. I also helped toby fix the workflow that updated 
the incubator stats: https://github.com/carpentries-incubator/carpentries-incubator.org/pull/6

#### Who helped you this week?

Toby helped me by showing me that setting up a bot is not as scary as I thought
it would be. Kevin Ushey helped me by acknowledging and fixing a bug in {renv}
https://github.com/rstudio/renv/issues/821.

#### What did you achieve?

* Created pull request to incorporate {renv} into {sandpaper}
  https://github.com/carpentries/sandpaper/pull/158
   - Demonstrated that it works in https://zkamvar.github.io/test-with-renv/
   - Tested rendering the above lesson on an old Windows machine with R 4.0.1
   - Added small vignette to demonstrate how to turn it on/off
     https://zkamvar.r-universe.dev/ui#view:sandpaper/building-with-renv.html
* Added styles-update script to two lessons in the incubator (maintained by
  Sarah Stevens)

#### What did you struggle with?

* Cache invalidaton
* Demonstrating the {renv} workflow in a vignette

#### What would you like to work on next week?

* start quarterly project plan for recruitment of the lesson infrastructure committee.
* merge {renv} pull request

#### Where do you need help from François?

As both Toby and I are dabbling in bots, I think it would be a good idea to
coördinate with Maneesha about creating an official carpentries bot account
similar to https://github.com/ropensci-bot

Things to consider for the bot account:
 - How do we control access with 2fa? 
 - Do we give it broad access for our organizations or do we make it repo-specific?
 - How often should we recycle tokens and who should be responsible?

#### Any other topics

I'm fairly happy with the solution I came up with for using {renv}. It does not
impose itself on users who have never used {renv} before, and it seems to work
well on continuous integration.

### Date: 2021-08-20

(written on 2021-08-23)

#### Who did you help this week?

I don't know that I helped anyone this week, TBH.

#### Who helped you this week?

Maxim helped me by reviewing the scope for https://github.com/carpentries/lesson-example/pull/350

#### What did you achieve?

* Completed workflow to update workflows: https://github.com/carpentries/sandpaper/pull/147
* Transferred the workflow actions to the Carpentries org: https://github.com/carpentries/actions/releases/tag/v0.4
* Update deployments chapter on the sandpaper documentation: https://github.com/carpentries/sandpaper-docs/pull/54
* Started working on a script to install/use dependencies in R Markdown lessons https://github.com/carpentries/sandpaper/blob/b40ae8c4794d0e92b85294508e1ae83afc2694e2/R/renv.R

#### What did you struggle with?

* Wrapping my brain around the right way to use {renv} has definitely been a challenge. It becomes really complex when you think about how to do this in a way that is minimally intrusive and allows for maximum reproducibility. 

#### What would you like to work on next week?

* start quarterly project plan for recruitment of the lesson infrastructure committee.
* Get a draft versio of package management with {renv}.

#### Where do you need help from François?

Nowhere at the moment! He's on vacation until the end of the month :sunglasses:

### Date: 2021-08-13

(written on 2021-08-16)

#### Who did you help this week?

I taught Instructor Training and also helped Talisha by recording attendance for
each day of IT. I also responded to a question about incorporating a python code
evaluation feature for the lessons. Finally, I helped the RStudio team by giving
feedback on quarto WRT jupytext.

#### Who helped you this week?

Maneesha, hands down, was the MVP. She stepped in for an hour each day of IT
when my co-instructor was unexpectedly away. Toby helped me come up with a plan
for planning the recruitment of the lesson infrastructure committee.

#### What did you achieve?

* Completed instructor training
* Refactored PR commenting to better explain what's going on: https://github.com/carpentries/sandpaper/pull/139
* Modularized CI deployment functions: https://github.com/carpentries/sandpaper/pull/144
* Migrated workflows to live inside of {sandpaper}: https://github.com/carpentries/sandpaper/pull/146
* Started workflow to update workflows: https://github.com/carpentries/sandpaper/pull/147

#### What did you struggle with?

* I think I struggled a bit with fetching branches in git, but nothing that has
  been insurmountable.

#### What would you like to work on next week?

* start quarterly project plan for recruitment of the lesson infrastructure committee.
* get a better sense of what can be accomplished with pull requests

#### Where do you need help from François?

Nowhere at the moment! He's on vacation until the end of the month :sunglasses:

#### Any other topics

The quarto demo looked promising! I think we might be able to use it to our advantage once we have our infrastructure set up. 

### Date: 2021-07-30

#### Who did you help this week?

I helped Erin find a green sticky in a red sticky regarding progress.

#### Who helped you this week?

François gave me good feedback about checking for links based on the review of https://github.com/carpentries/pegboard/pull/44.
Kelly, Danielle, and Erin helped me understand the expectations I should have for IT.

#### What did you achieve?

* JULY GOALS MET!!!
* merged first draft of link validator for pegboard https://github.com/carpentries/pegboard/pull/44
* fixed bugs associated with above validator to make it more flexible
* _heavily_ refactored the tests for {sandpaper} to use test fixtures https://github.com/carpentries/sandpaper/pull/134
* added in a message for episodes in draft https://github.com/carpentries/sandpaper/pull/135
* added lua filter to have a consistent cross-linking policy in the repository that should be robust to changes in our
  organisation of the untracked files (markdown and HTML) https://github.com/carpentries/sandpaper/pull/136
* added tests for git functions used by continuous integration https://github.com/carpentries/sandpaper/pull/137
* begun refactoring github workflows to allow for cron jobs and updates https://github.com/zkamvar/actions/pull/14
  (test repository at https://github.com/zkamvar/test20210729)
* prepared a little for the IT that I'm helping with on Monday and Tuesday

#### What did you struggle with?

* I struggled a bit with understanding what was expected of the lead trainer for the IT prep, but, as mentioned above, I was able to get help from people to better undertand it and calm my anxiety.

#### What would you like to work on next week?

* Instructor training and then a smol vacation

#### Where do you need help from François?

Nowhere at the moment

#### Any other topics

It was nice to have a week where I was only responsible for building things. Being able to sit down and think deeply about tasks like internal linking or testing really helped me come up with better solutions that work better in the long run. 

### Date: 2021-07-23

#### Who did you help this week?

I'm not sure I helped anyone but myself this week.

#### Who helped you this week?

Erin helped me by getting ad-hoc feedback from the maintainer community about my progression on the lesson infrastructure.

#### What did you achieve?

* finished and merged fix for heading validator for pegboard: https://github.com/carpentries/pegboard/pull/45
* finished first draft of link validator for pegboard https://github.com/carpentries/pegboard/pull/44
  * Note: this includes fixing of link handling in pegboard.
* Created two pull requests in the instructor training repository for broken links https://github.com/carpentries/pegboard/pull/44#issuecomment-885329710
* Refactored a whole lot of tests and messages in sandpaper https://github.com/carpentries/sandpaper/pull/133

#### What did you struggle with?

* I think I struggled a bit with getting CLI to play well with tests and not quite understanding that it was sending messages that could be suppressed.

#### What would you like to work on next week?

* Add feature to sandpaper to report informative messages to the users about episodes in draft
* Merge https://github.com/carpentries/pegboard/pull/44
* Get prepared for instructor training the first two days of the following week 😰

#### Where do you need help from François?

An approval of pegboard 44

#### Any other topics

It's been a WHILE since I updated this thing; In my defense, I was helping to teach instructor training, on vacation, at a conference, and my internet was in flux for two weeks during this period. 

### Date: 2021-06-04

#### Who did you help this week?

I helped Sarah Stevens by debugging an issue with a UMadison PR. The submitter
needed to update the branch against the main branch. 
I helped Maneesha and Kelly by volunteering for instructor training near the
end of June. 
I helped Karen by debugging a really weird issue on macOS: https://github.com/zkamvar/sandpaper-docs/issues/33

#### Who helped you this week?

Angelique, Karen, Erin, Maneesha, Kari, Shaun, and Caifan helped me by doing
user testing and interviews. 
François and Maneesha helped me understand how to get the born date of the
incubator repositories

#### What did you achieve?

* finished the outline for the useR talk
* started on the prose for the useR talk
* began data collection from alpha test interviews 
* completed five user testing interviews

#### What did you struggle with?

* I struggled a lot with writing the prose for the useR talk, but otherwise, the
  week seemed to go smoothly. 

#### What would you like to work on next week?

* Have slides templated by Friday
* Schedule a time in the Core team meeting on the 17th to present
* Address some of the backlog on my Asana

#### Where do you need help from François?

A better understanding of how we can use GitHub apps

#### Any other topics

I'm just really happy about how things are progressing.

### Date: 2021-05-28

(n.b. this was written on 2021-05-31, but only contains events until 2021-05-28)

#### Who did you help this week?

I helped Karen figure out a git issue that was blocking her work on testing out
the new lesson template on Friday.
I also helped Sher! with getting R set up on her Windows PATH. 
I finally found the issue that was blocking Sarah's progress on the UWMadison
data science curriculum (renv could not detect pacakges in block quotes).

#### Who helped you this week?

Toby helped me by helping Angelique get her git environment set up properly. 
François helped me by brainstorming ideas for the useR talk (and I still haven't
worked properly on it!). Jeroen helped me by letting me know that their GitHub
App setup costs nothing in terms of server time since everything is run via
GitHub Actions. This has big implications for Toby and I to create our bots.

#### What did you achieve?

* got a better idea of where I want to head with the useR talk
* added {textshaping} and {stringi} to our universe to avoid major headaches
* added support for reference links in {tinkr} and discussed implications of
  stripping namespace of document in object (this would heavily affect pegboard
  and require ~2 hours of refactoring). 
* Identified bugs in the lesson template 
* Attempted to convert the in-progress instructor training module. 

#### What did you struggle with?

* I struggled a lot with the useR talk. There is _so_ much that I could
  address, but i really need to focus on the audience (folks who would attend
  an R in Education talk/Educators) and choose a message (will it be the value
  of community feedback or the modularity of packages or a showcase of what you
  can do?)

#### What would you like to work on next week?

I'm noticing a pattern of things that I put on my agenda (token-based
authentication) that seem to be sticky and I can't shake. 

That being said, I would like to really nail down the narrative of my useR talk
especially since I have a short week this week. I want to have an outline of
slides and major talking points by Friday. 

#### Where do you need help from François?

A better understanding of how we can use GitHub apps

#### Any other topics

The template really is coming together nicely. Today, I spent some time working
with folks who did not have git + GitHub set up on their computer and I realized
that they all had the ability to install and use the template and that their
major hurdle was not the template, but rather working with GitHub. It's
promising because we would have these hurdles with Git _anyways_, but we have
significantly reduced the barrier for the lesson template. 

### Date: 2021-05-21

(n.b. this was written on 2021-05-23, but only contains events until 2021-05-21)

#### Who did you help this week?

I pointed a PR towards the styles repo that was updating OpenGraph for twitter cards. I also approved some PRs for glosario, but otherwise, I'm not sure that I _helped_ anyone per se. 

#### Who helped you this week?

- On the trend of the Alpha testing, I had four interviews this week and all of them really helped me understand some of the difficulties that would come up and how much this template will solve a lot of common problems.
- Maëlle always gives good reviews for my {tinkr} pull requests
- François merged my {glosario} updates.
- A few team members had scheduled Alpha test interviews, so I get to see it from their perspective :grin:

#### What did you achieve?

* Finshed four interviews
* got a shitty first draft of my talk (and I'm talking embarassing) at https://github.com/zkamvar/user2021
* added an R Universe for our Carpentries packages at https://carpentries.r-universe.org/
* drafted idea to use {tinkr} for preserving reference links, which will help with the migration of the instructor training, which _heavily_ uses these references links: https://github.com/ropensci/tinkr/issues/45
* Heavily revamped the setup page of the documentation site.

#### What did you struggle with?

* I had to take a mental day on Monday due to a lot of things going on in general, but other than that, I don't think I really struggled with much this last week. 

#### What would you like to work on next week?

Same as last week:

 - Since I didn't get to token-based authentication for GitHub workflows last week, I would like to do that this week
 - I would like to update the {sandpaper} documentation to accomodate the technical audience. 
 - I want to generate a rough outline for my UseR!2021 talk. 

But also:

 - I want to get a PR to tinkr that preserves relative markdown links.

#### Where do you need help from François?

Nothing this week!

#### Any other topics

None :D

### Date: 2021-05-14

(n.b. this was written on 2021-05-18, but only contains events until 2021-05-14)

#### Who did you help this week?

I'm not sure who I helped this week, exactly. I _attempted_ to help an incubator maintainer by proposing a fix to styles that allows BioConductor packages to be installed: https://github.com/carpentries/styles/pull/600, but the maintainer rolled their own in the end. I helped Dan figure out how to juggle tokens for GitHub so that he could propose changes to teaching git. It turns out pretty easy to add tokens and revoke them from GitHub's side, but removing tokens from your computer is a different matter. 

#### Who helped you this week?

- The participant in the alpha interview gave me good feedback from the perspective of someone who was extremely proficient at modifying their computational environment, but has never used R and had no desire to use R. They expressed the need for the documentation to be more clear up-front about what would be installed and more documentation related to exactlty _how_ the new lesson template engine worked. 
- Stefanie Butland posted a tweet that reflected my exact feelings about preparing for my UseR!2021 talk: https://twitter.com/StefanieButland/status/1393255336035815424

#### What did you achieve?

* I got one interview finished
* I attempted to update the {sandpaper} documentation based on user feedback (still in progress)
* I proposed a PR to styles that would allow for Bioc packages: https://github.com/carpentries/styles/pull/600
* I released the update to {tinkr} and made the `pegboard::Episode` class inherit from `tinkr::yarn`. 
* I found a way to enforce the main branch in new {sandpaper} repositories despite github versions: https://github.com/carpentries/sandpaper/pull/118'
* I updated the workflows for {sandpaper} to be better about caching and updating needed packages
* I modified the error message from {pegboard} when there was a fencepost error with the fenced div tags that is shown in https://github.com/zkamvar/sandpaper-docs/pull/28/files#diff-0307ac565dcb3ee031dffffe3cb97a6e8ac4cdf62b2f674dc0192461cdbd9be5R75
* I reviewed a PR that would add a twitter card to the template: https://github.com/carpentries/instructor-training/pull/1246

#### What did you struggle with?

* I struggled a bit with https://github.com/carpentries/styles/pull/600 and thinking how to accomodate the incubator maintainer who wanted the changes yesterday and the fact that the toolchain cascade requires careful reviews. The maintainer modified their own workflow, which involved changing permissions of the R library based on an incomplete mental model of how R libraries are used. There was a point where I realized that the maintainer's workflow was similiar to a former manager of mine and I ended up spiraling into anxiety, but that's beside the point. I think this all points to the fact that the toolchain cascade from styles -> carpentries-style -> incubator-template is not transparent and we need to at least document what we have right now so that it's clear how things can be updated before we move to the {sandpaper} engine. 

#### What would you like to work on next week?

 - Since I didn't get to token-based authentication for GitHub workflows last week, I would like to do that this week
 - I would like to update the {sandpaper} documentation to accomodate the technical audience. 
 - I want to generate a rough outline for my UseR!2021 talk. 

#### Where do you need help from François?

* A second pair of eyes on the glosario PRs
* Recommendation for what tutorials (if any) to take at UseR!2021: https://user2021.r-project.org/program/tutorials/ 

#### Any other topics

I'm really glad that I got the talk secured for UseR!2021 and now am a bit nervous about it (of course) because I am slightly paranoid that I overpromised in the abstract, but I know that I have _too much_ to talk about and that's definitely a good place to be in.

### Date: 2021-05-07

#### Who did you help this week?

I helped Maëlle with a [PR in {tinkr}](https://github.com/ropensci/tinkr/pull/39), I also helped Karen by submitting a [pull request to fix all http links](https://github.com/data-lessons/instructor-training/pull/68) in her update of instructor training. People at the CT meeting also found my skillup session on GitHub pull request things.

#### Who helped you this week?

- François helped me by having a discussion around the scope of our automation and trying to figure out when we would actually need to release an app or bot.
- The participant for the Alpha interview gave some very good feedback on the language used in the instructions and said that it was going in a good direction.

#### What did you achieve?

* I got one interview finished
* I updated the {sandpaper} documentation based on user feedback
* I proposed a PR to update {tinkr} to allow for protection of math blocks and github tick boxes
* I found a [method of including alt text without forcing people to using RMarkdown](https://twitter.com/ZKamvar/status/1390357892893601792)
* I opened two infrastructure PRs in glosario: https://github.com/carpentries/glosario/pull/319 and https://github.com/carpentries/glosario/pull/312
* I fixed a bug in {pegboard} https://github.com/carpentries/pegboard/pull/34
* I got the converter to work (so far) for the python novice gapminder lesson

#### What did you struggle with?

* I think I mainly struggled with prioritizing things and feeling guilty for working deeply on problems that were not immediately useful (like {tinkr})

#### What would you like to work on next week?

Next week, I may be sick for the first day or two, so it will be a shorter week. I am to work further on {sandpaper} documentation, making sure that {pegboard} is compatible with the new version of {tinkr}, and exploring token-based automated updates via github actions. 

#### Where do you need help from François?

* A second pair of eyes on the glosario PRs

#### Any other topics

There's a lot of legacy kipple that has accumulated over the years. I had thought that the maintainer onboarding was a new project from Erin and Angela last year, but given Dan's questions, I looked at the repository again and now understand how long it's been around. I think one of the things I'm realizing is that I really need to make sure my documentation is absolutely solid (which includes philosophy and justification) so that it can continue on when I'm no longer around.

### Date: 2021-04-30

(N.B. This was written on 2021-05-03)

#### Who did you help this week?

I helped Dan, Toby, and Erin by reviewing Dan's proposal to the maintainer community. I also helped on the {tinkr} repository by templating code for protecting math blocks.

#### Who helped you this week?

- Erin, Toby, and Daniel really helped me a lot by speaking frankly about maintainer community organizing. 
- Michael tried out the previous lesson template and gave me his impressions of it. 
- One of the participants in the Alpha test gave me a lot of feedback on the installation process that was very helpful.
- James Balamuta helped me understand that GitHub Apps needs a dynamic webserver in order to work :/

#### What did you achieve?

* I got one interview finished
* I updated the {sandpaper} documentation based on user feedback
* I came up with an idea of how to allow bare brackets to be processed in {tinkr}

#### What did you struggle with?

* I struggled a lot with trying to figure out how exactly GitHub Apps actually work and understanding that I had an incorrect model of where the code was running. 
* I also struggled with trying to understand how to provision a workflow to accept 

#### What would you like to work on next week?

Same as last week:

* I would like to get the workflow for the installation laid out and pulled
* Fixes to the {sandpaper} documentation

#### Where do you need help from François?

* Discussion of the pros and cons of the update workflow in the new template.

#### Any other topics

Growth phase of an organization is always hard, especially considering that we are a volunteer-based org. Every day I come to work, I try to keep in mind that the work I do is explicitly in service to the community so that I can make their lives easier so that they can focus on the volunteer effort they are doing for a cause that they care deeply about. 


### Date: 2021-04-23

#### Who did you help this week?

Thinking of this week: I helped a bunch of people, I think. I helped Maxim by reviewing and merging several pull requests. I helped Erin by giving advice for the Astronomy lesson, and I helped Toby by talking deeply about the maintainer community situation.

#### Who helped you this week?

Toby and Daniel really helped me a lot by speaking frankly about maintainer community organizing. Michael and David also really helped by giving really detailed feedback on the alpha test of the lesson template. Kelly helped me by stepping in for instructor training when Luca was sick. 

Again, the entire curriculum team was REALLY helpful in being super supportive of me during the Alpha phase of the lesson template

#### What did you achieve?

* Sent instructions for alpha-phase of lesson template to the participants
* co-lead bonus module instructor training for online workshops
* had two interviews for the Alpha phase
* created a github workflow that will update the styles of lesson-example every week: https://github.com/carpentries/lesson-example/pull/340
* brainstormed way of addressing the installation issue (but haven't yet implemented)
* restarted converter script

#### What did you struggle with?

* I struggled a lot with the maintainer RFC situation and also the instructor training bonus module. I have been really stressed this week, TBH

#### What would you like to work on next week?

* I would like to get the workflow for the installation laid out and pulled
* Fixes to the {sandpaper} documentation

#### Where do you need help from François?

* Instructions on how he keeps the lessons using remote theme up-to-date

#### Any other topics

I was really glad to talk with David and Michael. They both were enthusiastic in very different ways and both had positive experiences despite bugs. It was good to end the week on a good note work-wise, but I think the events of the week have definitely impacted everyone and we need to take care to support each othe. 

### Date: 2021-04-16

#### Who did you help this week?

Thinking of this week: I helped Dan by posting the announcement for the upcoming mainters meeting on Topicbox. I helped Maxim by fixing a bug in a python function and making a PR to update the lesson example. I helped Erin by responding to a query about the two urls for CDH. 

Over the past two weeks, I have done several styles updates for astronomy python, one HUGE one for python-socialsci, and lesson example. 

#### Who helped you this week?

Toby, Erin, and François helped me out a lot by running with the pre-alpha testing of the new template and identifying pain points in the instructions (e.g. it doesn't make sense to have people use git through R quite just yet). I also really appreciate François helping out with deeper discussions of the lesson template and the testing strategy.

Dan Chen really helped me by reiterating the struggles people have with getting R to work on Windows.

#### What did you achieve?

* got the pre-alpha phase of testing with the Curriculum Development Team done and out of the way
* tested the new template on an old windows laptop from both RStudio and the command line
* fixed a couple of annoying bugs in {sandpaper}
* sent out recruitment email to potential alpha testers and got back eight positive responses so far

#### What did you struggle with?

* I struggled with a couple of things. One thing I struggled with was finding the right words to describe the alpha test to the testers. I also struggled with corectly scoping the tasks for the new template, and I especially struggled with the maintainer RFC suggesting for the lead maintainer status. I was mostly struggling to stay focused on task this week for some reason.

#### What would you like to work on next week?

* I would like to send out the alpha test to the people who responded affirmatively and brace myself for impact

#### Where do you need help from François?

* Not sure yet.

#### Any other topics

One of the things that I've been thinking about is what the maintainer community is and thinking about how its structure is similar or dissimilar to other communities outside of The Carpentries. The strife that's being expressed in the RFC is nothing new and it's understandable. At this moment, each maintainer operates their own lesson in their own particular way and feels empowered to make important decisions about that lesson based on feedback in issues and pull requests. The suggestion of implementing a superstructure to the lessons feels like a threat to their independence. It's like telling an rOpenSci package maintainer that they must have a representative for their package report every year. I think there is a way to do a bottom-up approach to organizing, but we need to get more people engaged because at the moment, there are a few voices downing out the others.

### Date: 2021-03-31

#### Who did you help this week?

I don't think I helped anyone in particular this week. 

#### Who helped you this week?

I had an interview with Al after the Core Team meeting that allowed me to think about the role of our maintainers in the broader scope of our institutional partnerships. 
Kari jumped on a call with me to help remind me how to assign multiple tasks in Asana. 
François helped me by reminding me that expressing emotions because of my work is okay and it is not considered whining. 
Toby helped me by talking through the salient points of what needs to be tested in the Alpha phase of the lesson template testing.

#### What did you achieve?

* identified a bug in {usethis} and missing documentation in {gert} where git config options were normalized and caused a "main" branch to never be created: https://github.com/r-lib/gert/issues/133
* created first draft of Alpha testing for lesson template (definitely still in progress)
* reviewed draft 2 of the Hi-Fi wireframes
* clarified some details of work for frontend developer

#### What did you struggle with?

* I struggled _a lot_ with communication differences between myself and the UX designer, which arises from thier ethic to deliver only finalized products and adherance to the written statement of work (e.g. sharing notes was not on the statment of work) competing with my ethic to work openly. I don't think they are wrong, I just regret that we did not anticipate this situation.

#### What would you like to work on next week?

* I would like to finalize the Alpha phase draft after getting feedback from the Curriculum Team

#### Where do you need help from François?

* A push to communicate more broadly about items in work to keep me accountable with the community.

#### Any other topics

I've been thinking about all the support I've been given over the past year and I'm just so grateful that I get to work with this team. I know it sounds corny, cheesy, or some other foodstuff descriptor that indicates a feeling of sentimentality (no one ever says that's hella cabbage, though and they really should), but I've only had one other manager in my life that's been as supportive as François has been. I think about all the difficulties that have been thrown at us and how we have been able to face each of them and figure out how to handle these situations. We have such a wonderful, caring, and resiliant community that anyone who interacts with them notices. I am still finding the challenge of creating the new template, well, challenging, but I know that whatever I come up with will be a step in the right direction and the feedback I get from the volunteers will help guide my path. 

### Date: 2021-03-23

#### Who did you help this week?

I helped a lot of people with their pull requests and got several of the R
lessons updated with the current version of styles.

#### Who helped you this week?

A lot of people helped me. Most prominently, Erin, François, Toby, Scott Chamberlain, and Maëlle Salmon helped me by reviewing my submission to UseR!2021. Erin helped me understand my frustrations about the UX design. 

#### What did you achieve?

* I have a fully functional lesson template taht can go from zero to working GitHub site with minimal setup.
* I have updated the first episodes in https://zkamvar.github.io/sandpaper-docs
* I merged a bunch of PRs in styles
* I reviewed the designs of the new lesson template front end

#### What did you struggle with?

* I think I struggled with communication differences in the UX design, mostly. I sometimes still think of the size of this project and realize how much is left to be done. 

#### What would you like to work on next week?

* I would like to finalize the list of maintainers to alpha test the template and finalize the documentation.

#### Where do you need help from François?

* Nowhere since he's on vacation

#### Any other topics

It's been a month and I've definitely made some progress toward the goals, but the revelation last month that I wasn't going to be able to make my deadline was a bummer and it helped to push it back. I actually had to push it back further because I realized in the middle of my retreat that we wouldn't have things ready in time as the documentation site was coming together like a sloppy joe. 


### Date: 2021-02-23

#### Who did you help this week?

I don't recall helping anyone, TBH

#### Who helped you this week?

François and Toby helped me understand that the lesson template project needed to be pushed back. 

#### What did you achieve?

* I presented the tentative lesson template plan to a small group of maintainers who were able to attend the maintainer meetings. The idea was recieved well.
* I figured out the basics for creating nested templated data in https://github.com/zkamvar/grosbeak#readme, but still haven't really figured out how to use it to smooth out the monstrosity of moving files around in the lesson template. 

#### What did you struggle with?

* Prioritizing tasks and communication. I think the lesson template rollout was really stressing me out on top of the ambiguity I was feeling from the initial wireframes. I realized that there were many places where we should have had better communication: with the designer of what the important points of the template were, with the participants of what the scope of the interviews were for. I struggled a lot with differing working styles between myself and the designer. I felt conflicted giving piecemeal feedback inside of figma (which was a struggle in and of itself---I really the lack of navigational control I have in that program), when a holistic approach was needed. I felt like I was always in catch up mode.

#### What would you like to work on next week?

* It's.... difficult to tell. I think since I'm going on vacation next week, I'm going to spend the rest of this week fixing small issues and prioritizing things that I can 

#### Where do you need help from François?

* I really don't know. 

#### Any other topics

It's been a real struggle

### Date: 2021-02-16

#### Who did you help this week?

THAT'S A QUESTION I WOULD LIKE TO KNOW (read: no one)

#### Who helped you this week?

Emily's research helped me understand some of the pain points of the lesson template.

#### What did you achieve?

* I set up https://zkamvar.github.io/sandpaper-docs/
* I wrote a lot of junk
* I dispared
* I added a bunch of issues to {sandpaper}, {pegboard}, and {varnish}

#### What did you struggle with?

* LOL EVERYTHING

#### What would you like to work on next week?

* I'm supposed to announce to the maintainers that the Alpha testing will commence in March, but IDK man, things are looking pretty bleak (hey that's what happens in midwinter, my brain gets all sorts of cuckoo bananas).

#### Where do you need help from François?

* Lots, but not sure where to start.

#### Any other topics

Get better!

### Date: 2021-02-09

#### Who did you help this week?

This last week was largely focused on instructor training. I found that my brain was oatmeal by the end of it, and I wasn't really able to be of much help to anyone other than the learners and my coinstructor. 

#### Who helped you this week?

Karen definitely helped me as I was in the throes of utter dispair due to my porridge menenges.
François, Toby, and Erin helped give me feedback on the tutorial submission for UseR!2021

#### What did you achieve?

* Taught instructor training
* Submitted UseR! tutorial
* Add fixes to {sandpaper} that renders the index.md and allows for bare uris and emoji (https://github.com/carpentries/sandpaper/pull/68 and https://github.com/carpentries/sandpaper/pull/71)
* Created a drat repository https://carpentries.github.io/drat/

#### What did you struggle with?

* OATMEAL BRAIN

#### What would you like to work on next week?

* I would like to close all of the issues for the alpha phase testing: https://github.com/carpentries/sandpaper/milestone/5

#### Where do you need help from François?

* Nowhere at the moment!

#### Any other topics

Karen is a saint for being able to listen to me complaining about oatmeal brain so much.

### Date: 2021-02-02

#### Who did you help this week?

I helped Toby by updating his suggested change describing the build process for R lessons on the lesson-example repository.

#### Who helped you this week?

François came through in a big way by sifting through the lesson template plan and getting an initial draft of the alpha goals in addition to updating the roadmap in the sandpaper repository. This really helped me understand the priorities better.

#### What did you achieve?

* presented my work to the Core Team: https://docs.google.com/presentation/d/1MloMSt8cumfCmoobH_sLfNqEifex3BhbGN0DJfU1KKA/edit?usp=sharing
* tested the current [lesson template transformation process](https://github.com/zkamvar/new-programming-with-r/blob/95592dced88878199554708690401eade70ab378/instructors/migration-notes.md), identifying pain points along the way.
* addressed some bugs in the current template that was based on naïve assumptions about how pandoc treats HTML blocks: https://github.com/carpentries/sandpaper/pull/65
* Added a change to {varnish} to [allow styling of level 3 headers in callout blocks](https://github.com/carpentries/varnish/commit/64b3d707061acb7df008549a40e30cb9d6ab3151).
* Fix several new bugs in {pegboard}: https://github.com/carpentries/pegboard/pull/21

#### What did you struggle with?

* I definitely struggled with parsing kramdown syntax: https://github.com/carpentries/pegboard/pull/21/commits/02e879812a077cb2653dcc2a146a935aa27ed8c4

#### What would you like to work on next week?

* Polish up rollout plan (clarify what constitutes success for each phase)
* Create submission drafts for UseR! 2021 (both tutorial and talk)
* First Instructor Trainer workshop (AAAAAAH!)

#### Where do you need help from François?

* At the moment, I'm not sure what I need, but that seems to be a recurring pattern :disappointed:.

#### Any other topics

I'm definitely doing better than I was one week ago. I think a lot of factors helped: the time I took off, the time spent at the reading and reflection day, the excercise of forming my ideas about the template into a presentation, and documenting the conversion of a lesson into the current template.  

### Date: 2021-01-26

#### Who did you help this week?

I don't think I really helped anyone this week. 

#### Who helped you this week?

Last week was short and hazy as I took sick time for most of Thursday and Friday,
so it's hard to remember

#### What did you achieve?

* Created a rough idea of what the path forward should be regarding the lesson template rollout with François (deadline: tomorrow/today :grimace:)
* Contributed to hiring decisions

#### What did you struggle with?

* LOL Everything

#### What would you like to work on next week?

> NB: this is copy-pasted from the previous week because I was in over my head.

* Finish the first draft of rollout plan.
* Create fork of an R-based repository to test out the GitHub Actions.
* Create communication outlines for each step of rollout plans (contact Omar).
* Investigate how to properly write tests for the GitHub Actions.

#### Where do you need help from François?

* Still nebulous

#### Any other topics

I suffered from anxiety last week and I think one of my takeaways is that I don't feel comefortable asking for help because I feel like everyone on the CurrTeam already has a full plate. At this point, because much of my work has been tinkering without much community input, it's hard to identify places that I need help that wouldn't also require a big time commitment from the other team members.

### Date: 2021-01-19

#### Who did you help this week?

* I helped François by fixing a bug in the feeds where the label colors were not being processed: https://github.com/carpentries/feeds.carpentries.org/pull/47.

#### Who helped you this week?

* Erin helped me when I was taking notes during the interviews by stepping up when I had gotten flustered at the beginning.

#### What did you achieve?

* Incorporated my [GitHub Action to close a temporary branch](https://github.com/zkamvar/actions/tree/main/remove-branch#readme) in my test repository: https://github.com/zkamvar/testme/commit/18854c595291c390b1f6c2424e8ac8d8557d11dc, which reduced the complexity of the origingal workflow by over 50 lines.
* Created several diagrams of the lesson components that are in https://zkamvar.github.io/stunning-barnacle/
* Begun the process of outlining the Rollout plan (see [Rollout.md](./Rollout.md) or https://zkamvar.github.io/stunning-barnacle/rollout.html).
* I participated in three interviews for two positions on our team.
* Added substantive content to Emily's onboarding document.

#### What did you struggle with?

I believe I struggled with trying to tie all of the little parts of the rollout plan into a bigger picture. This on top of trying to balance the hiring committee interviews and dealing with an unexpected interruption on Thursday made me feel like I wasn't able to get much done in the last week.

#### What would you like to work on next week?

* Finish the first draft of rollout plan.
* Create fork of an R-based repository to test out the GitHub Actions.
* Create communication outlines for each step of rollout plans (contact Omar).
* Investigate how to properly write tests for the GitHub Actions.

#### Where do you need help from François?

* Nowhere concrete at the moment.

#### Any other topics

While I was working on compiling information Emily needed for the redesign of the template, I came upon several posts from 2014 about the redesgin of the lesson template:

 - https://software-carpentry.org/blog/2014/09/splitting-the-repo.html
 - https://software-carpentry.org/blog/2014/10/new-lesson-template-v2.html
 - https://software-carpentry.org/blog/2014/10/of-templates-and-metadata.html
 - https://software-carpentry.org/blog/2014/10/yet-another-template-for-lessons.html
 - https://software-carpentry.org/blog/2014/12/templates-we-live-we-learn.html
 - https://software-carpentry.org/blog/2015/06/updating-the-lesson-template.html
 - https://software-carpentry.org/blog/2016/07/rmarkdown-new-template.html

I wish I had thought to look these up earlier, because they give a lot of needed persepective and shows what people were thinking about when they were initially designing the lesson template. 

As always, I tend to fret over minor things outside of our control. I need to remember to focus on our goals and what we can explicitly control (the user interface) and what is out of our control. For example, I want to make sure that we do not stray too far from the RStudio publishing ecosystem (Blogdown, Pagedown, etc), but at the same time, there are some design decisions, limitations, and features that do not align with our goals.

I'm realizing that one of the biggest friction points for us is that designing an enigine for a blog and designing an engine for a lesson template are similar in the sense that you want to give people a way of sticking in markdown and getting a website out of the other end; but they are different because of **who is responsible for managing workflow and aesthetic decisions**. For a personal blog, the onus on choosing the brand and keeping everything up to date is on the author and if the ecosystem shifts, they can choose to shift with it or switch to something else. This case is not too difficult if it's just one or two blogs that they maintain. In the case of a lesson template, we have hundreds of lessons that need to have the same or similar branding and need to be robust to changes in the software ecosystem. 


### Date: 2021-01-11

#### Who did you help this week?

I helped folks in the Maintainer Community Coworking Corral answering questions about updating styles. For example, I helped Sarah Stevens get her capstone project updated so that RMarkdown documents would automatically build.

#### Who helped you this week?

Omar, Erin, Kari, and Talisha helped this week by reminding me that it's okay to take a break from work during times of national strife.

#### What did you achieve?

* I have created three github actions and written a rationale for them in https://github.com/zkamvar/actions/#readme
* I updated the action that comments on PRs to ammend its comment instead of creating new comments (similar to Netlify)
* I was able to create a Pull Request workflow that will fail early if the pull request is invalid: https://github.com/zkamvar/testme/actions/runs/473399683
* I found a really good article about i18n for static sites: https://www.smashingmagazine.com/2020/11/internationalization-localization-static-sites/ (which goes into serverless redirects via Service Workers [client-side JS that lives on the user's machine and is associated with a single origin]). 

#### What did you struggle with?

* As always, I struggled a lot with GitHub Actions and JavaScript. Specifically, I struggled trying to find the balance

#### What would you like to work on next week?

* I would like to complete my action suite by introducing an action that removes the PR branch, completing the task that I assigned to myself before the break. 

#### Where do you need help from François?

* Should we consider deploying the auto-building, staging, and commenting on the Pull Requests soon before we release the new template? I think it would be good to see how the maintainers would interact with bots commenting on their pull requests. 

#### Any other topics

After reading the article about [i18n for static sites](https://www.smashingmagazine.com/2020/11/internationalization-localization-static-sites/ ), I'm thinking about our abstraction model for the lesson template. The reason that we have it set up the way we do at the moment is conforming to Jekyll's standards of how a website should be laid out. We've taken this into consideration and reformed the folder structure to better accomodate the lesson structure itself and hid the site generating machinery from the maintainer. There are a couple of problems, though:

 1. My plan for folder structure organization is fragile. I don't currently have a good abstraction model for it and it will break if the backend of the site changes.
 2. As laid out in [i18n and l10n for static sites](https://www.smashingmagazine.com/2020/11/internationalization-localization-static-sites/), this is _hard_, like really difficult. At the moment, I don't think {pkgdown} or {rmarkdown} handle this well.
 
One of the things I need to focus on is figuring out a good way to create a generic map for what the maintainers see to what any given static site generator will expect (e.g. {rmarkdown}/{pkgdown} expects flat structure, {blogdown} expects a Hugo structure). Once we have that, we can find the generation mechanism that will work for us and deploy it.
 
 
### Date: 2021-01-05

#### Who did you help this week?

No one! Nobody was around :)

#### Who helped you this week?

Scott Chamberlain helped me with BASH and [Colin Fay helped me understand JS](https://twitter.com/_ColinFay/status/1344662815274053637?s=20) problems when trying to debug https://github.com/zkamvar/check-valid-pr

#### What did you achieve?

 * I have created a few GitHub workflows:
   - Receive Pull Request and build diffs
   - Create orphan branch comparing PR with built branch
   - Comment on PR with diff/link to PR
   - Remove temporary branch once PR is closed
 * I have created a GitHub action that validates an incoming Pull Request, checking if it modifies workflow files or if it tries to spoof a closed PR:  https://github.com/zkamvar/check-valid-pr
 

#### What did you struggle with?

* I struggled a lot understanding security vulnerabilities via the actions.
* I also had a hard time figuring out when to switch languages (e.g. JavaScript was MUCH better at interacting with the GitHub API than BASH).
* JavaScript :/

#### What would you like to work on next week?

* Document the Workflows I have set up
* Create a plan for new Actions to be created

#### Where do you need help from François?

* Do the workflows make sense (after I document them)?

#### Any other topics

It was good to be able to put myself into this part of the work where I would have to fail a lot and be juggling several processes at once. I think the first part of December didn't allow for much of that because I was working on a lot of interviews and meetings.

