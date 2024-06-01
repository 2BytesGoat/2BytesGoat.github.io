---
tags:
  - learn-ai
date: 2024-06-01
---

In the past people used to analyze a problem and come up with complicated rules (think of the video game bots). Building up these rules would take developers years to develop and perfect. 

Nowadays, we can use techniques such as machine learning where we throw a agent into the "world" and let it struggle until it "learns" how to exploit the game. 

The downsides:
* based on how you will reward your AI, it may "learn" some behavior that will maximize it's rewards but it may not behave like you want it to - [See Video Example](https://www.youtube.com/watch?v=L_4BPjLBF4E)
* the AI will need to interact with a environment or humans for it to learn
* it's not always possible to understand why it took certain actions - which may be vital for applications such as autonomous driving

# The questions you need to answer

As Obi-Wan once said, [only a Sith deals in absolutes](https://www.youtube.com/watch?v=kVu_yMEhUfM), which in our case translates to there are more than 2 ways to build an AI. 

Here are some questions you can answer that will help you determine how to build an AI:
* How much time do you have to build it?
* Do you any way to get examples from an expert performing the task?
* Do you want to understand why the AI took a certain action?
* Do you have any hardware restrictions when deploying the AI?
* Is it ok for the the AI to produce a action every 2-3 seconds or do you need it to "think" faster?

I can come up with more, but I think answering those will be a good indicator for the type of AI you can build.

# Practical example

> [!example] Hypothetic Scenario
> Say you're making a personal project where you want to build an AI capable of classifying ~~tweets~~ posts on X as being either offensive or not.

You have multiple ways of doing it:
## 1. ask ChatGPT
You can make a call to the OpenAI API and ask chatGPT to classify your post as either offensive or not offensive.

**Pros**
- you can probably build it in a afternoon
- you don't need to know anything about Machine Learning
- you don't need to know or use a programming language like Python
- you can tweak how sensitive it can be to offensive posts through prompting

 **Cons**
- it may classify the same post differently if you ask it multiple times
- you won't be able to use your AI if ChatGPT is down
* you'll need to pay for a subscription 
* you won't know why ChatGPT did something even if you ask it

## 2. build a Machine Learning Classifier
You can train an AI using [Machine Learning]([[What is Machine Learning]]) by feeding it a lot of examples with what you mean with offensive and not offensive.

**Pros**
* the AI will know exactly what you mean when you call a post offensive
* you can determine what are the cases the AI does good or needs more data
* you can obtain some reasoning for why the AI took a action
* you could deploy the AI on your own custom hardware
* the AI should be able to answer in under 1 second
* you'll probably need to know Python or C++

**Cons**
* you need to create a training dataset that will be used to train the AI
* you need to have the resources and time to train and refine the AI
* you need to know which AI backbone to use, and implicitly some knowledge of Machine Learning
* it's going to be harder to upload based on what hardware you have
## 3. build a Rules-Based System
You can create a set of rules such as a list of bad words or users that usually post offensive things on social media. 

**Pros**
* you have full control over the AI
* you can trace down the exact steps it went through in order to get to a answer
* you can always update/upgrade how it behaves
* it's very light weight and fast
* it can be done in any programming language
* can be uploaded on a potato

**Cons**
* it's a iterative process and will take a lot of trial and error
* it's hard to capture nuances of the language (slang, synonyms etc.)
* you'll need to think of the rules and come up with solutions for problems by yourself

# Outro

That was a long one... hope you found it useful tho 😊

If you want to learn more, but don't know where to go next? Try one of these paths:
* [[What is Machine Learning]]
