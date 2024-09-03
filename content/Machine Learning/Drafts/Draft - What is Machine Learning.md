---
tags:
  - learn-ai
draft: true
date: 2024-06-01
---
**M**achine **L**earning, broadly speaking, means that you can give a computer some examples of a behavior you want it to learn, and it will come up with a formula that models that behavior. 

## Why machines need to learn
Let's say your PC just gave birth to a new baby AI 👶. Congratulations! From the start, the baby will know nothing about this world. The baby will then need examples to learn from and a way to check that what it learns is desirable. 

> [!Note]
> The way a Machine Learning model can figure out how far it is from the desired example and optimize the way it thinks is called a `loss function`
## How a machine learns
I briefly mentioned the `loss function` and the fact that it helps your ML baby to learn. Let's get a bit more technical. 

Let's say you have images of cats and racoons and want to make a Machine Learning model that can tell them apart. Your dumb ML baby that knows nothing about the world will need to make a prediction for each image: Is this a cat or a racoon? It's almost impossible for the ML baby to know from the get-go to tell them apart (hence it knows nothing about the world). That means that it will make mistakes.

We then need a way to communicate to the ML baby that it made a mistake and how to correct itself. Here comes the `loss function`. It will help us compute the error between what it said and what it should have said and it's also `derivable` which mean that the ML baby can learn how to update itself.

You run this experiment a few times and hopefully the now ML model will not learn all the examples by-heart and it will actually know to generalize once you show it a new picture of a racoon. 

> [!Note]
> I mentioned that the loss function should be `derivable` in order for a ML model to learn from. That's because a ML model is made out of a bunch of numbers, that all impact the accuracy of it's predictions. 
> 
> If you hear scary words such as `partial derivative`, all it means is that it calculates how much a certain parameter of the ML model impacts the output. Was this number the reason my prediction was bad? How much should I change it? The answer: based on the `partial derivative` and `learning rate`. 

## What is a foundation model
Similarly to how we grow up, go to school and are exposed to a lot of varied experiences, that shape the way we look at the world, we can do the same with a machine learning model. What happens is that the ML model will learn about a lot of information (literature, math, chemistry etc.) without necessarily it being a expert in the field. We can then either guide or fine-tune the model in order for it to fit our needs. 

> [!Note]
> The reason we build foundations models is both: 
> * because we can just feed them whatever data we have at hand
> * because it can figure out relationships between domains that would otherwise would imply more work to separate

## What does fine-tuning mean
To put it simple, fine-tuning is the process of specializing a already trained machine learning model on a specific task. 

For example, you can have a machine learning model which is generally good at up-scaling images no matter the contents, and you specialize it to be excellent in up-scaling images with people, such that you can use it to restore old pictures your grandma took in 2002.

> [!Note]
> Usually when you fine-tune a model that is generally good on a specific task, you will lose it's generality. 
> 
> Meaning that if it was good at math, chemistry and physics and you want it to only be good at complicated math problems, it will forget how to chemistry. 

## Outro
Hey 👋 In case it's your first time delving into the realm of Machine Learning and AI in general, maybe you'll be interested in some short side quests to make you feel less confused.
* [[Draft - What does AI even mean?]] 
* [[Draft - Why building an AI is hard]]
