# 🛠️ Fine Tuning Workshop 🎯

Hello, world! 🌍 Let's talk about the magic of fine-tuning! Ever wanted GPT-3.5 to give you code, precisely how you like it? You're in the right place! We're diving deep into how to fine-tune our friend, GPT-3, to get more precise code outputs. 🚀

## 📌 Table of Contents

1. [What's the Goal?](#whats-the-goal)
2. [Setting Things Up](#setting-things-up)
3. [The OG Prompt](#the-og-prompt)
4. [Gathering Our Training Data](#gathering-our-training-data)
5. [Model Upload Time!](#model-upload-time)
6. [The Moment of Truth: Testing!](#the-moment-of-truth)

<a name="whats-the-goal"></a>
## What's the Goal? 🎯

We've got a mission! 🕵️‍♂️ Instead of long, windy prompts, we want to shoot GPT-3 a concise one and get back sweet, sweet code in this format:
```
[filename.ext]
```code
CODE HERE
```
```

Sounds cool, right? 🤩 Let's get started!

<a name="setting-things-up"></a>
## Setting Things Up 🛠️

First things first, let's make sure we've got all our tools ready. 

Install the magic potion with:
```bash
pip install --upgrade openai
```

And then, let's summon our trusty sidekicks:
```python
import json
import openai
import os
import glob
```

<a name="the-og-prompt"></a>
## The OG Prompt 📜

Remember the OG (original) prompt? Yep, it was a bit of a chatty one! 🙊 We're on a mission to make it shorter, sweeter, and more to the point!

<a name="gathering-our-training-data"></a>
## Gathering Our Training Data 🎒

Alright, time to gather our training data! It's like prepping ingredients for a delightful recipe. 🍲 Our `example_data` folder has got the goodies. We'll use this as our base for training GPT-3.

Quick magic spell to grab all our data files:
```python
files = glob.glob("example_data/*")
```

And then, it's transformation time! 🦋 We'll get these files ready for training.

<a name="model-upload-time"></a>
## Model Upload Time! 🚀

Alright, fam! Once we have our data ready, it's time to give GPT-3 a little training session. Imagine it as a mini bootcamp! 🏋️‍♂️ We'll do this at OpenAI's platform: https://platform.openai.com/finetune

<a name="the-moment-of-truth"></a>
## The Moment of Truth: Testing! 🎉

Alright! Moment of truth! After that mini bootcamp, it's time to see how well GPT-3's been trained! Let's test our fine-tuned model and see the magic happen! 🌟

---

Happy coding and fine-tuning! Remember, with every iteration, we get closer to perfection! 🌈🎈🎉

## Need data?

Checkout hugging face, they have over 70,000 datasets that you can use for fine-tuning.

https://huggingface.co/datasets