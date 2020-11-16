# Meeting Notes

## Table of Contents
 
 - [2020-11-17](#date-2020-11-17)
 - [2020-11-10](#date-2020-11-10)
 - [2020-11-04](#date-2020-11-04)
 - [2020-10-21](#date-2020-10-21)

### Date: [INSERT DATE OF MEETING]

#### Who did you help this week?

Replace this text with a one/two sentence description of who you helped this week and how.


#### Who helped you this week?

Replace this text with a one/two sentence description of who helped you this week and how.

#### What did you achieve?

* Replace this text with a bullet point list of what you achieved this week.
* It's ok if your list is only one bullet point long!

#### What did you struggle with?

* Replace this text with a bullet point list of where you struggled this week.
* It's ok if your list is only one bullet point long!

#### What would you like to work on next week?

* Replace this text with a bullet point list of what you would like to work on next week.
* It's ok if your list is only one bullet point long!
* Try to estimate how long each task will take.

#### Where do you need help from François?

* Replace this text with a bullet point list of what you need help from François on.
* It's ok if your list is only one bullet point long!
* Try to estimate how long each task will take.

#### Any other topics

This space is yours to add to as needed.


### Date: 2020-10-17

#### Who did you help this week?

IDK if I really helped anyone. 
We had a productive meeting today with Toby and Kari to discuss the presentation for CZI, but otherwise, I don't think there's much I did to help anyone else.

#### Who helped you this week?

Erin helped me a lot by answering my pesky questions about the evaluations. 
Toby and Francois helped me by [providing ideas on a folder structure for {sandpaper}](https://github.com/zkamvar/sandpaper/issues/22).

#### What did you achieve?

* I finished the evaluations for most of the members of the core team
* I made a [pull request in {sandpaper} that adds in extra folders to the lesson contruction](https://github.com/zkamvar/sandpaper/pull/25)
* Kari, Toby, and I came up with an outline for the talk at CZI in December

#### What did you struggle with?

Surprisingly, I [struggled](https://github.com/zkamvar/sandpaper/pull/25/commits/ff66dc752d95fa81f4f2c4934f3111471eab9f08) [a lot](https://github.com/zkamvar/sandpaper/pull/25/commits/5f0f1c857127a10b08a23202a32142eb0b6e7616) [with paths](https://github.com/zkamvar/sandpaper/pull/25/commits/6bbda285324c24ac7a848c129c8320fd6b76f071) [in {sandpaper}](https://github.com/zkamvar/sandpaper/pull/25/commits/0380a64c403fd3086ab65d75a30e35467a2f0569).
I realized that I was attempting to over-complicate things by assuming that I should allow people to define separate paths for the lesson outputs, which would cause me numerous headaches when it came to juggling paths, especially with subprocesses and copying artifacts.
At the moment, it's still inflexible to the ordering of folders and to what folders are detected, but it appears to work. 

#### What would you like to work on next week?

* I would like to incorporate the lua filter that transforms `instructor` tags into `<aside>` tags into the build process. (that's all I will have time for since there are a buttload of meetings and reviews this week. 

#### Where do you need help from François?

* I've moved the `Setup.html` resource into the `For Learners` dropdown to reduce the real estate. Is this okay? 

#### Any other topics

I remember you mentioning that you wanted to go with a style of lesson where we have dual sidebar navigation.... which looks like what "bs4_book" from bookdown has: https://r4ds.had.co.nz/tibbles.html. There's a good discussion about the style of this format here: https://twitter.com/daattali/status/1321561642329608201


### Date: 2020-11-10

#### Who did you help this week?

I don't know that I helped anyone in particular. Maybe Bailey Harrington by editing her PR to Glosario, but then again I did mess that up a bit... :weary:
I think I helped Christophe Dervieux by demonstrating how I'm subverting RStudio tools for my own nefarious purposes. He was able to see how scope creep is affecting the ecosystem (case in point, {pkgdown} was never intended as a generalized website builder).

#### Who helped you this week?

Maëlle Salmon helped my by critiquing my PR for {tinkr} and also giving perspective about the limitations of {tinkr} vs other methods of editing a markdown document (may turn into blog post). 
Christophe Dervieux helped me by pointing out areas in the infrastructure that have alternative or even better solutions (e.g. since we are working with markdown, we could be relying on pandoc's AST instead of commonmark). 

#### What did you achieve?

* Added an {R6} object to {tinkr}: https://github.com/ropensci/tinkr/pull/33
* Created this repository
* Addressed a HUGE PR in Glosario: https://github.com/carpentries/glosario/pull/187
* Thought (and slightly dispaired!) about changes to the infrastructure for the new lesson template: https://github.com/zkamvar/sandpaper/issues/23, https://github.com/zkamvar/sandpaper/issues/22
* I began work on my performance review

#### What did you struggle with?

* I struggled a lot with the idea that a lot of the work I've been doing over the past few months on {sandpaper} may result in a bit of a dead end because the tooling I've chosen was inappropriate. That being said, I've spoken a bit more with Christophe and I think there is a way forward.

#### What would you like to work on next week?

* I need to finish my performance evaluation
* I will update the CSS in {sandpaper} and investigate methods for creating the downloadable code snippets taking into account the functionality of [Sara Brown's magic snippets](https://raw.githubusercontent.com/carpentries/carpentrycon/master/CarpentryCon-2018/Sessions/2018-05-30/08-Lightning-Talks-Session-2/brown-poster.pdf) (reference on [Jupyter Magic](https://ipython.readthedocs.io/en/stable/interactive/magics.html)).

#### Where do you need help from François?

* For the code snippets, I understand that these should effectively be code files, with the challenge text as commented markdown. The question is: where will these live? My opinion is that they should live in the repo website branch and not the staging branch since they are effectively duplicates of the content that exists in the episodes.

#### Any other topics

As I'm coming to the cusp of realizing that I need to switch the internal method of creating the website, I've been thinking a bit about Rework Avoidance Theory and how that's been impacting my work: https://twitter.com/GeePawHill/status/1296122333099417600.

### Date: 2020-11-04

#### Who did you help this week?

I helped Talisha and Sher! by fixing a ruby bug in GitHub Actions in Library Carpentry that prevented the data from being updated https://github.com/LibraryCarpentry/librarycarpentry.github.io/pull/110 

#### Who helped you this week?

Toby helped me by merging the above pull request and pointing out that you had already done the same thing with the main site.

#### What did you achieve?

- I’ve completed the first draft of the Landscape overview
- I’ve created a pull request in {tinkr} to give it an R6 class that makes adding elements to the XML document easier. 

#### What did you struggle with?

I struggled a bit with not being distracted yesterday and today...

#### What would you like to work on next week?

I expect to work on bits of {tinkr}, {pegboard}, and the {sandpaper} template
given the changes outlined in the [Landscape](Landscape.md) document. I estimate
migrating the changes in {tinkr} should take less than a day, {sandpaper} should
take around a day because I will have to rearrange the folder structure, and 
{pegboard} will be ongoing because the change in {tinkr} changes the paradigm of
how I move around the XML object and make modifications.

#### Where do you need help from François?

Coming up with ideas for using the EIA funds.

#### Any other topics

None!

## Date: 2020-10-21

## Who did you help this week?

This is a morally ambiguous question because the concept of help is subjective on the person receiving help.

- Batool Almarzouq - I helped her by figuring out how to get directionality incorporated into glosario
- Annajiat Alim Rasel - I helped him by reinforcing where he should report errors for the lesson template.

## Who helped you this week?

- Batool Almarzouq helped me by pointing out that the text she submitted was flipped with my initial implementation of the direction attribute.
- Daniel Chen stepped in for me in the maintainer meeting.

## What did you achieve?

- A lot of my work this last week was focused on reading a lot to try and understand xml2 namespace handling and how I should best use that for {pegboard} and {tinkr} (which turns out to be a lot)

## What did you struggle with?

- I struggled a lot with trying to figure out what I need to focus on with the lesson template development. {sandpaper} is important, but making sure that {tinkr} and {pegboard} are functional is also key. 
- I struggled to understand how JSON-LD was implemented

## What would you like to work on next week?

Since it’s on the curriculum team list, I would like to get a plan for the github action for our lesson sorted out. I have https://github.com/zkamvar/glowing-chainsaw/blob/main/episodes/extras/deploy.R, which I blatantly stole from {pkgdown}, and I just need to implement it in a github action. 

## Where do you need help from François?

- I need to bounce ideas off of you about the scope of https://docs.google.com/document/d/1XfzZd2L00TduC8XeAPL-Z6Dhaj1xJZBY5vwT2mb-gjw/edit?disco=AAAAHEtoeGA 
  - Do this at rendering time and store in subfolder with link.
- Extra files: 
  - Think about dropdown menus with extra content (anchored to carpentries, but specified)

## Any other topics

Lesson metadata: where should it live?

## Notes

- Transfer some code from pegboard to tinkr and make sure Maëlle is on board with it
  - Create R6 object for tinkr, add basic functionality (adding new node based on Markdown text)
  - Release of tinkr also depends on testthat 3 being released


- Where are the specifications going to live? Vignettes?
  - For the specifications we need to decide what we are going to present to the users and in which order
  - First thing is a fully formed lesson with at least 2 episodes
    - Organization
    - Building and Deployment (how do i get the thing from my computer to the web)
    - Episode structure
    - Pro tips and pitfalls
    - Validation
  - Come up with realistic mistakes users might make and ensure that they fail the validation.
    - First step: write specification document for people (not machines). 
    - Document in codimd
    - Remember: start with specifications in september deliverables
    - Concept map 
    - Write up the document from there
    - Use our blog post from July
  - Linking in the context of i18n….

