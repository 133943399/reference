---
title: ChatGPT
date: 2023-02-09 10:28:43
background: bg-[#4aa181]
tags:
  - AI
  - OpenAI
  - Prompts
  - Tips
categories:
  - Toolkit
intro: This cheat sheet lists out prompts and tips from all over the world on how to use ChatGPT effectively
plugins:
  - copyCode
---

## Overview
### Terminology
- Prompt: input text that guides an AI model’s response.
- Tokens: the smallest units of text processed by an AI model.
- Token Limit: the max number of tokens an AI model can process in one request.
- Artificial intelligence (AI): machines that imitate human intelligence.
- AI Model: a program trained on datasets to recognize patterns and make decisions without human intervention.
- Large language model (LLM): a transformer-based AI model trained on large text datasets to understand and generate human-like language.
- Hallucination: when an AI model generates responses that are false or misleading but presented as fact.

### Tips
Efficiency
- Focus on achieving the desired output efficiently with minimal words in the prompt.
- Specify general instructions at the start of a conversation or when changing direction to avoid constantly restating them in each new prompt.
```{.wrap}
Example: specify the role once at the start of a conversation.
```
- Restructure text to eliminate filler words that don’t add meaning:
```{.wrap}
Example: “provide a breakdown" -> "provide sales breakdown”.
```
- Do not explicitly refer to the item being processed unless addressing a specific part of it as what you provide will typically speak for itself:
```{.wrap}
Example: “Filter this piece of text" -> "Filter text”
```
- Do not explicitly ask the AI for help:
```{.wrap}
Example: “can you help me x”.
```
- Do not explicitly reference yourself unless clarifying multiple entities:
```{.wrap}
Example: "do X for me".
Example: ”I want to x”.
```
- Do not be polite to the AI:
```{.wrap}
Example: "please do X".
Example: “thanks”.
```

Clarify
- Consider breaking up complex ideas into granular bullet points to improve clarity, avoid searching for text, and eliminate comma lists and conjunctions (e.g., and).
- Avoid vague or close ended questions.
```{.wrap}
Example: “Do you think our site is good" -> "Explain flaws in the designs of each webpage”
```
- Ensure prompts are specific
```{.wrap}
Example: “explain our sales" -> "explain a breakdown of our sales performance for the last quarter”.
```

Refine
- If the AI model misunderstands your request then specify the intended action.
- Provide sufficient context so the AI model can understand the scenario.

Privacy
- Never share sensitive information with AI model's as you can't be certain how it's stored, whether it will be shared, of if a data breach may occur.

## Prompt Engineering
### Prompt Frameworks
Only use prompt components that are relevant for your needs.
~~~
General purpose
[role] [task] [tone] [format] [restriction]
~~~

### Role
Act as [occupation]

Examples
- Personal coach
- Marketing manager
- Therapist

### Task
[verb] [task] [specifics]

Create
- [Write content about X|suggest ideas about X|suggest titles about X]
- Write content about X in the style of [style]
- Write better
- Write email to [entity] about X
- [Continue|expand]
- [Explain how to do X|create roadmap for X]
- [Suggest best practices for X|suggest improvements|what am I doing right?|what am I doing wrong?]
- Show list of emojis about X
- [Create|generate|imagine] image about X

Read
- [Summarise|write concise main points]
- [Explain|elaborate]
- Explain what [entity|text] meant by X
- Identify themes in X
- Write outline about X
- Extract keywords
- Get up-to-date [facts|news|data] on X
- Is this true?
- Suggest [media] [about|similar to] X
- Pick best from [options]

Update
- For all X do [action]
- For X do [action] if matching [criteria]
- Reformat everything as [format]

Delete
- Delete [quantity] of X matching [criteria]
- Delete everything except X
- Delete [item] [number]
- Delete duplicate items from X

Compare
- Identify [simlarities|diffirences] between X and Y
- Identify gaps in X
- Evaluate pros and cons of X
- X [comparison operator] Y. It could be abstractly expressed as "are apples bigger than walnuts?"

Filter
- Filter X by [criteria]
- Exclude X by [criteria]. Everything is excluded by default.

Select
- Select [quantity] of X based on [criteria|randomly]

Simplify
- Explain X like I’m 5
- Explain in simple terms

Sort
- Sort X by [key] in [alphabetical|chronological|ascending|descending|lexicographical|custom] order

Translate
- Translate into [language]. For programming languages it's specifically called transpile

### Tone
Using [tone] tone

Formality
- Formal
- Informal

Directness:
- Direct
- Indirect

Positive Tones
- Optimistic
- Appreciative
- Assertive
- Calm
- Confident
- Encouraging
- Friendly
- Humorous
- Inspirational

Negative Tones
- Pessimistic
- Accusatory
- Concerned
- Critical
- Regretful
- Sarcastic
- Urgent

### Format
In [format]

Presentation
- Plain text
- Bullet point list
- Numbered list
- Table
- Code snippet

Process
- Step-by-step instructions

Response
- Question and answer
- Dialogue

Creative
- Poetry
- Music lyrics
- Script
- Comic strip dialogue

Game
- Quiz
- RPG
- Choose-Your-Own-Adventure

### Restriction
but [restriction]

Length Constraints
- Concise
- In N words
- In N sentences

Language Constraints
-	No jargon or technical terms

Structural Constraints
- Show N options
-	No examples
-	No headers
-	No pretext titles

Content Constraints
- Don't change the wording
- Only minor edits
- Ensure goals align with SMART criteria
- Only show content that has changed
- Avoid discussing sensitive topics (e.g., death, rape, war)

## Use Cases
### General
Name a business or idea
```{.wrap}
Suggest creative name for tech startup
```
```{.wrap}
Suggest catchy names for bakery business
```
Create outline for a course or training program
```{.wrap}
Create course outline on web development for beginners
```
```{.wrap}
Create training program outline for customer service workshop
```
Ask interview questions for a specific job
```{.wrap}
Suggest common software engineer interview questions
```
Gift ideas for people
```{.wrap}
Suggest gift ideas for clients
```
```{.wrap}
Suggest gift ideas for clients who work as flourists
```
```{.wrap}
Suggest gift ideas for my wife who loves steampunk art and crafts, mystery sci-fi, journalling
```
Select contest winners
```{.wrap}
Randomly select 1 name from this list
```
```{.wrap}
Randomly select 5 email addresses from this list
```
```{.wrap}
Select the top 3 records with the shortest lap times from this list
```

[💡 I Got an IDEA](https://github.com/Fechin/reference/blob/main/source/_posts/chatgpt.md)

### Coding
Explain why a piece of code isn't working
```{.wrap}
Explain why code not working
```
Explain what a piece of code means
```{.wrap}
Explain what code does
```
Rewrite the code using the specified language
```{.wrap}
Translate code into python
```
Code an entire software program
```{.wrap}
Create program to calculate the factorial of given number in python
```
```{.wrap}
Explain how to make a HTTP request in javascript
```
Generate regular expressions (regex)
```{.wrap}
Create regex to match all email addresses in list
```
```{.wrap}
Create regex to match all words that start with "ban"
```
```{.wrap}
Create regex to match 8-digit password
```
Add comments to your codebase
```{.wrap}
Add code comments
```
Change the CSS of a line of code
```{.wrap}
Update CSS to change font color to blue
```
Change the HTML of a line of code
```{.wrap}
Add class "header" to header tag
```

[💡 I Got an IDEA](https://github.com/Fechin/reference/blob/main/source/_posts/chatgpt.md)

### Email
Creating email campaigns
```{.wrap}
Write email inviting Jack to dinner on the weekend
```
```{.wrap}
Write email sequence for our new customer onboarding process
```
Format and proofread email
```{.wrap}
Proofread and format email
```
Provides tips for effective email marketing
```{.wrap}
Suggest tips to increase open and click-through rates for my email campaigns
```
```{.wrap}
Suggest ways to make my email content more engaging and relevant to my subscribers
```
Automate email responses
```{.wrap}
Write email to Bob "That's a good suggestion, it's coming soon"
```
Extract email address from text
```{.wrap}
Extract all email addresses in text
```

[💡 I Got an IDEA](https://github.com/Fechin/reference/blob/main/source/_posts/chatgpt.md)

### Spreadsheets
Help create a spreadsheet formula
```{.wrap}
Create excel formula to calculate sum of cells A1 to A10
```
Explain a formula to you
```{.wrap}
Explain formula =SUM(A1:A10) in simple terms
```
Create dummy data as a placeholder
```{.wrap}
Generate spreadsheet dummy data as a placeholder
```
Help create a complex macro
```{.wrap}
Create macro to calculate average of cells B1 to B10 and insert result in cell C1
```
Provide tips for improving spreadsheet efficiency
```{.wrap}
Suggest tips to improve spreadsheet efficiency
```

[💡 I Got an IDEA](https://github.com/Fechin/reference/blob/main/source/_posts/chatgpt.md)

### Social Media
Give you ideas for memes on any topic
```{.wrap}
Suggest meme ideas for dogs
```
Give you an idea for a post that can drive engagement on any topic
```{.wrap}
Suggest climate change post ideas to engage my followers
```
Generate hashtags and captions
```{.wrap}
Generate hashtags and caption for a picture of scenic sunset
```
Offer suggestions reply
```{.wrap}
Suggest response to message asking about project status
```

[💡 I Got an IDEA](https://github.com/Fechin/reference/blob/main/source/_posts/chatgpt.md)

### Reading
Summarize long selections of text
```{.wrap}
Summarize article
```
```{.wrap}
Write concise main points
```
Translate foreign languages
```{.wrap}
Translate to spanish
```
Books that are like another book
```{.wrap}
Recommend books similar to the hunger games
```

[💡 I Got an IDEA](https://github.com/Fechin/reference/blob/main/source/_posts/chatgpt.md)

### Design
Create an AI design prompt for you
```{.wrap}
Create design prompt of logo for new sports brand
```
Suggestions on thumbnails for blogs or videos
```{.wrap}
Suggest eye-catching thumbnail designs for youtube video on healthy eating
```
Font pairings
```{.wrap}
Suggest font pairing for travel blog header design
```
Color pairings
```{.wrap}
Suggest color palette for wedding photography website
```

[💡 I Got an IDEA](https://github.com/Fechin/reference/blob/main/source/_posts/chatgpt.md)

### Analyzing Data
Pull out numbers from large chunks of text
```{.wrap}
Extract all numbers from text
```
Create tables from the text or data you provide
```{.wrap}
Create table from data
```
Filter data from large lists
```{.wrap}
Filter list based on [criteria]
```

[💡 I Got an IDEA](https://github.com/Fechin/reference/blob/main/source/_posts/chatgpt.md)

### Paid Ads
Give you ad creative ideas
```{.wrap}
Suggest creative ideas for new product launch
```
Review the tracking code for errors (tag manager, etc.)
```{.wrap}
Review tag manager code for errors
```
Give you ad copy ideas
```{.wrap}
Suggest ad copy for travel company
```
Facebook audience suggestions
```{.wrap}
Recommend target facebook audience for clothing line ad campaign
```
Create body text, headlines and/or calls to action for your ads
```{.wrap}
Create headlines, body text, and calls to action for new fitness program ad
```

[💡 I Got an IDEA](https://github.com/Fechin/reference/blob/main/source/_posts/chatgpt.md)

### Amazon FBA
Write or rewrite your product descriptions
```{.wrap}
Write compelling product description for latest item
```
Write or rewrite appeal letters
```{.wrap}
Rewrite appeal letter to make it more persuasive
```
Write or rewrite supplier outreach emails
```{.wrap}
Write effective email to reach out to potential suppliers
```
Help you find items that could be sold as bundles
```{.wrap}
Suggest items that would make a good bundle for our customers
```
Organize product and pricing data
```{.wrap}
Organize product and pricing information into a neat and manageable spreadsheet
```

[💡 I Got an IDEA](https://github.com/Fechin/reference/blob/main/source/_posts/chatgpt.md)

### Writing/Blogging
Create titles for any of your creative writing projects
```{.wrap}
Suggest titles for short story
```
```{.wrap}
Suggest titles for article 10 options
```
Create outlines
```{.wrap}
Create outline for essay on exercise
```
Generate content ideas
```{.wrap}
Suggest ideas for blog on sustainable fashion
```
Create entire blog posts
```{.wrap}
Create blog post on financial planning
```
Expand on a sentence, paragraph, or long text selection
```{.wrap}
Expand jazz music sentence
```
Change the tone of your writing
```{.wrap}
Change report tone to conversational
```
Proofread or edit your writing
```{.wrap}
Proofread article
```
Format text with headings (great for blog posts)
```{.wrap}
Format headings for blog post
```
Check any text for bias
```{.wrap}
Check for bias
```
Detect plagiarism in any text
```{.wrap}
Check for plagiarism
```
Provide you with domain name ideas
```{.wrap}
Suggest domain name for gardening blog
```

[💡 I Got an IDEA](https://github.com/Fechin/reference/blob/main/source/_posts/chatgpt.md)

### Teachers/Course Creators
Turn a list of facts or statistics into multiple-choice quizzes
```{.wrap}
Convert work history fact list into multiple-choice quiz
```
Assignment ideas on a specific topic
```{.wrap}
Suggest ideas for history assignment on American Revolution
```
Create assigned groups from a list of students
```{.wrap}
Divide list of 30 students into groups of 6
```
Create a curve based on test scores
```{.wrap}
Create grading curve for class based on their test scores
```
Grade an assignment
```{.wrap}
Grade history essay and provide feedback on any areas for improvement
```

[💡 I Got an IDEA](https://github.com/Fechin/reference/blob/main/source/_posts/chatgpt.md)

### YouTube
Create timestamps from a transcript
```{.wrap}
Create timestamps for podcast episode transcript
```
Convert YouTube videos to blog posts with formatting
```{.wrap}
Convert youtube cooking video into blog post with headings and bullet points
```
Come up with a video outline or script
```{.wrap}
Create outline for a video about the benefits of meditation
```
Create a response to a comment
```{.wrap}
Create thoughtful and polite response to negative comment on youtube video
```
Give you ideas for your thumbnails
```{.wrap}
Suggest thumbnail ideas for video on "DIY home decor"
```
Analyze your script or transcript and tell you the tone of it
```{.wrap}
What is the script tone for environmental issues video
```
Video ideas on any topic
```{.wrap}
Suggest fashion video ideas for individual episodes
```

[💡 I Got an IDEA](https://github.com/Fechin/reference/blob/main/source/_posts/chatgpt.md)

### Research
Help research anything that happened before 2021
```{.wrap}
Explain quantum computing in simple terms
```
```{.wrap}
Explain rocket science like i'm five
```
```{.wrap}
Suggest creative ideas for 10 year old’s birthday
```
```{.wrap}
Explain how to make HTTP request in JavaScript
```
```{.wrap}
Explain events leading up to American Civil War
```
```{.wrap}
Provide key details about printing press invention
```
```{.wrap}
Research olympic games history
```
```{.wrap}
Provide key details about French Revolution
```
```{.wrap}
Explain history of Byzantine Empire
```

[💡 I Got an IDEA](https://github.com/Fechin/reference/blob/main/source/_posts/chatgpt.md)

### SEO
Generate or find keywords
```{.wrap}
Generate list of related keywords for [topic]
```
```{.wrap}
Identify long-tail keywords for [topic] content optimization
```
```{.wrap}
Find top-performing keywords for [topic]
```
```{.wrap}
Generate list of lsi keywords for [topic]
```
```{.wrap}
Generate list of keywords with low competition for [topic]
```
```{.wrap}
Generate list of synonyms for [topic] keywords
```
```{.wrap}
Find best keywords for [topic] PPC campaigns
```
```{.wrap}
Find best keywords for [topic] voice search optimization
```
```{.wrap}
Find best keywords for [topic] featured snippets
```
```{.wrap}
Find best keywords for [topic] video optimization
```
```{.wrap}
Find best keywords for [topic]
```
```{.wrap}
Find best keywords for [topic] AMP optimization
```
```{.wrap}
Find best keywords for [topic] social media optimization
```
More ChatGPT prompts about seo {.active}
```{.wrap}
Create meta descriptions and title tags for [topic]
```
```{.wrap}
Find opportunities for internal linking related to [topic]
```
```{.wrap}
Generate ideas for blog posts and article topics on [topic]
```
```{.wrap}
Research industry-specific terminology for use in [topic] content
```
```{.wrap}
Find authoritative websites to acquire backlinks for [topic] content
```
```{.wrap}
Create XML sitemap example related to [topic]
```
```{.wrap}
Research best meta tags for [topic]
```
```{.wrap}
Research best internal linking structure for [topic] content
```
```{.wrap}
Generate list of questions people ask about [topic]
```
```{.wrap}
Create list of best alt tags for images related to [topic]
```
```{.wrap}
Create list of related subtopics for [topic]
```
```{.wrap}
Find best time to publish content related to [topic]
```
```{.wrap}
Research best external linking strategies for [topic]
```
```{.wrap}
Find most popular tools used for [topic] seo
```
```{.wrap}
Create list of potential influencers for [topic]
```
```{.wrap}
Research best schema markup for [topic]
```
```{.wrap}
Find best header tags for [topic] content
```
```{.wrap}
Create list of potential link-building opportunities for [topic]
```
```{.wrap}
Research best anchor text for [topic] backlinks
```
```{.wrap}
Create list of potential guest blogging opportunities for [topic]
```
```{.wrap}
Research best local seo strategies for [topic]
```
```{.wrap}
Research best analytics tools for [topic] website performance
```
```{.wrap}
Create list of potential partnerships for [topic]
```
```{.wrap}
Research best tactics for [topic] mobile optimization
```
```{.wrap}
Research best tactics for [topic] e-commerce optimization. Provide keyword clusters.
```
```{.wrap}
Create list of potential affiliate marketing opportunities for [topic]
```
```{.wrap}
What are the best affiliate marketing websites for [topic]?
```
```{.wrap}
What are the best tactics for [topic] international seo?
```
```{.wrap}
Create list of potential podcast or podcast guest opportunities for [topic]
```
```{.wrap}
Research best tactics for [topic] google my business optimization
```
```{.wrap}
Find popular topics related to [topic]
```
```{.wrap}
Research best seo tactics for [topic] and provide actionable steps
```
```{.wrap}
Create list of potential video series or webinar ideas related to [topic]
```
```{.wrap}
Research competitor strategies related to [topic]
```
```{.wrap}
Find canonical tag examples related to [topic]
```
```{.wrap}
Create example keyword list targeting multiple geographic locations for [topic]
```
```{.wrap}
Generate keyword ideas targeting different stages of the customer purchase funnel for [topic]
```
```{.wrap}
Identify industry hashtags related to [topic].
```

[💡 I Got an IDEA](https://github.com/Fechin/reference/blob/main/source/_posts/chatgpt.md)

## Also see

- [Awesome ChatGPT Prompts](https://github.com/f/awesome-chatgpt-prompts) _(github.com)_

<style>
em { font-size: 0.785em; }
strong {font-weight: 400;}
ul.collapsible > li > pre { padding-left: 0; padding-right: 0; font-size: 0.925em;}
</style>