+++
title = "What is Actually Going On"
description = "Cognify - A Fake Website for a Real Idea"
date = "2023-06-29"
aliases = ["real", "realtalk"]
author = "Hugo Authors"
+++

# This is for a Class Project

This website was created as an assignment for the Northwestern Masters in Data Science program, for the 431 - Intro to Go class.  More details can be found TKTK HERE.

### Assignment Prompt

*Personal knowledge base products tap into a need we all have: to organize our ideas over time. We read something and make a note of it. We read something else and make another note. We see that things are related and make a note of that as well. At one time or another, everyone has used a Google KeepLinks to an external site. or Microsoft OneNoteLinks to an external site.. Memo-makers and note-keepers opened the door to personal knowledge bases. ObsidianLinks to an external site. walked through that door, moving further along. They see that the power isn't in the individual notes, but in the links between the notes. To foster creativity and productivity, we need a kind of mind-map or graph database of ideas. But Obsidian, as currently defined, has limited potential. What user in the general public knows Markdown, which is needed for formatting the Obsidian notes? And why ask the user to manually enter links between ideas when AI can do it automatically? We can do better than Obsidian, and we have the technical savvy to pull it off.*

ASSIGNMENT TKTKTKTK

### An Actual Approach

Building a system like this is relatively straightforward, although it's not easy.  You need the following pieces to build an AI linking engine:

1. Your folder of Obsidian notes.  These notes can be anything from quick jots of thought to notes on books to full articles that have been imported into markdown.  There can be rich text, code, video, pdfs, etc in them
2. A process for extracting key concepts from files.  The whole notion of identifying themes or key concepts is a class in and of itself (and here's a link to the Northwestern MSDS-453 Intro to Natural Language Processing, and here's my github repo for that class).  Let's just take as a given that this work can be done
3. A user front-end to scan through suggested links and allow the user to vote yea or nay for which links are real
4. A parser that can go through the markdown notes and insert the deep links necessary to map notes together.

So you're looking at a simple file folder structure, some python code for natural language processing, javascript or node.js for a front-end interface, and then go for fast processing and editing of the files.

### So This Website is... Unbelievably Stupid-Sounding

Yeah.  It is.  The focus of the assignment was to create a website using Hugo themes (this was built in Hugo Up Business theme.  It's great), with content being an afterthought.  I figured I'd have some fun with it by letting AIs develop a website about AI.

#### ChatGPT Prompt

I gave ChatGPT the following prompt:

I have the following prompt from which I need to make a website.  Don't worry - I'm not asking you to do my homework.  I'm looking for you to provide something a little more sophisticated and funnier than using lorem ipsum.  Here is the prompt:

**Prompt from above**

Now what I need is the text in the website.  I need it to be as over-the-top as possible.  I need the following sections:

1. In the homepage:
   1. A hero description.  A bold heading with a line or two of text.  Please suggest a hero image description that I can go find myself
   2. The three key concepts that are part of this offering.  Each concept has a bold heading with a 3-4 sentence description of why the concept is amazing.  Same deal: need a description of an image to go with it
   3. Three testimonials.  I need the testimonials to be embarassingly gushing and I need the names to be punny

2. An "About our Offering" section.  This should be three paragraphs long, with three hero images that look impressive but are totally unrelated

3. An Our Team page.  Five individuals.  I want their experience to be dumb and unrelated to anything coding related

4. A pricing page.  I need you to create a table that has various potential service offerings, with three tiers of pricing.  Each tier should have a random assortment of included / excluded features.

I want all of this over-the-top, filled with buzzwords.  This needs to be jargony and dense while also sounding impressive.  Thank you!!!

#### ChatGPT's Response

I used ChatGPT's response more or less verbatim in the rest of the website.  The one thing that I found hilarious was the image descriptions that ChatGPT suggested.  I took the descriptions and copied them verbatim into StableDiffusion and selected the most appropriate image.

The biography page similarly relied on AI to create profile pics for each of the company's leaders.  So if you zoom in and realize that someone is missing a hand, that's why.