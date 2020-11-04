# Meeting Notes

## Table of Contents

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

