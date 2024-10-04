# README

This exercise aims to help us understand your approach to building software with Rails.

# Getting started

To get the Rails server running locally:

- Clone this repo
- bundle install to install all required dependencies
- rails assets:precompile to install tailwind assets
- rails s to start the local server

## In scope

The goal is to enable you to demonstrate how you do the following:

- Write tests
- Write code
- Create components
- Name methods
- Structure commits
- Write commit messages
- Consider performance (if appropriate)

## Out of scope

- Making this a full end-to-end application with user logins, security etc. It's just to provide space for you to create models, views, controllers, components and specs to demonstrate the above
- Deploying to staging or production environments
- Setting up linters like Rubocop

## Brief

Please create a form for a clinician to write clinical notes in response to a series of questions. Each question should be mapped to one Autism DSM IV criterion.

In a separate view, for a given completed form, group the questions and their responses by DSM criteria to allow the clinician to read the notes they've taken for each criterion.


**Example data**

Questions and written Notes (notes are filled in by the user)

| number | question  | notes |
| ------ | --------- | ----- |
| 1 | Social verbalization/chat | The client demonstrated some social use of speech in response to caregiver |
| 2 | Reciprocal conversation | Occasional reciprocal conversation, but less frequent than normal or limited in flexibility and topics |
| 3 | Imaginative social play | Some pretend play, including actions directed to dolls or cars etc., but limited in variety or frequency |
| 4 | Use of other's body to communicate | Some more notes written by clinician A |
| 5 | Pointing to express interest | you get the idea |

DSM criteria grouping of questions

| key | description | mapped_numbers |
| --- | ----------- | ------ |
| A1 | Deficits in social-emotional reciprocity | 1,2,3 |
| A2 | Deficits in nonverbal communicative behaviours used for social interaction | 4, 5 |


**The form**

The form to collect the notes should have the questions in linear order and the ability to submit them along with entered notes for each question

**The view**

The view should group the entered questions by DSM e.g. for example showing data in the following tables but styled nicely

A1 - Deficits in social-emotional reciprocity

| No. | Question | Notes |
| --- | -------- | ----- |
| 1 | Social verbalization/chat | The client demonstrated some social use of speech in response to caregiver |
| 2 | Reciprocal conversation | Occasional reciprocal conversation, but less frequent than normal or limited in flexibility and topics |
| 3 | Imaginative social play | Some pretend play, including actions directed to dolls or cars etc., but limited in variety or frequency |

A2 - Deficits in nonverbal communicative behaviours used for social interaction

| No. | Question | Notes |
| --- | -------- | ----- |
| 4 | Use of other's body to communicate | Some more notes written by clinician A |
| 5 | Pointing to express interest | you get the idea |



