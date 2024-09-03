---
tags:
  - learn-ai
draft: false
date: 2024-09-03
---
# TL;DR

<details>
	<summary>Lesson Summary</summary>
	<p>Loss Functions (also known as Error Functions) are used to calculate how far a AI behaviour is from a expected behaviour. The AI uses the result of the error function to take a step in the right direction. There are multiple error functions because each function is better for a given task the AI needs to be better at. </p> 
</details>

# Your Quest

Quests are here to provide some purpose for having to read through the theory. Read the quest and figure out how the information below can help you complete it.

> [!warning] The Quest for the Wakewine
>Read the post to figure out what Error Functions are to find your way to the nearest _café_.
> 
> - Understand Mean Squared Error
> 
> - Understand Mean Absolute Error 
> 
> <big>**Description**</big>
> 
> **The Day of Conquest has arrived!** The long-awaited moment to master the arcane arts of machine learning is upon you. Yet, one important matter must be addressed.
>
>With unwavering determination, you rush towards the kitchen. However, the sight that greets you is beyond belief. “Unacceptable!” you shout. “One does not simply acquire knowledge cafeineless!”
>
>You take a deep breath to steady yourself. "Luckily, there are two coffee shops nearby", you say to yourself. But now, you must decide: **Which one will you choose?**
> 
> <big>**Rewards**</big>
> 
> You will receive: 
> 
> - 📜 **The Scroll of Error Functions**

# What are Loss Functions

Let's say a friend of ours, Roger, asks us whether we want to go to a coffee shop we've never been before. However, Roger's a bit of a douche and only answers with "hot" if we're closer or "cold" if we're further from the shop.

Thus, without knowing how far exactly we are, we start walking while asking Roger how close we are every step of the way. The moment he'll scream "boiling hot", we know we got to the destination. Thus concluding our journey from point A to B for our coffee.

A similar thing happens with Machine Learning. The only difference is that A represents how the AI behaves right now and B is how we want it to behave. And we quantify the difference between how it behaves and how it should behave with a **Loss Function** (also known as **Error Functions**).
# Squared Distance


# Absolute Distance

