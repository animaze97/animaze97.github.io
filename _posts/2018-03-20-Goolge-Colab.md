---
layout: post
title: Introduction To Google Colab
bigimg: /img/1.jpeg
tags: [Machine Leaning, Deep Learning, Google Colab, Colaboratory]
---

If you are a machine learning newbie, I am sure you might have run into the giant obstacle of — “Where to train my models?” Don’t worry, Google has you covered. Google released its internal research tool “Colaboratory” which is a tool for machine learning education and research. It’s a Jupyter notebook environment that requires no setup to use. In simpler terms, it’s a jupyter notebook with all the collaboration abilities of Google docs, meaning more than one person can work on the same code at the same time. But, the real attraction is the free computing power that this tool offers.

Google colaboratory currently offers the computing services of a Tesla K80 GPU for free. Yeah, you heard that right -“free”. The only catch here is that you can use the computing services for a maximum of 12 hours at a time (you can think of it in terms of a session). Basically, when you train your models on the colaboratory, you are connected to a GPU-based virtual machine where you are given a maximum of 12 hours at a time, after which you lose access to that particular virtual machine instance (all data, that is, models parameters as well as datasets that aren’t saved to the Google drive before this period will be lost, so make sure to save snapshots of your model parameters at regular intervals, else you will have to start training your models from scratch again). After 12 hours you are assigned a different virtual machine (for free of course) and the cycle repeats. There’s no limit for how many virtual machines can be used through one account, so “Train” to your heart’s content.

To select the GPU for training you need to go to: Runtime > Change runtime type or Edit > Notebook settings, from there you can select the python version as well as the Hardware accelerator (GPU) for training.

image: /img/2.jpeg

Its way simpler if you have worked with jupyter notebook before, if not, you can explore around a bit to get the hang of it. Working with Colaboratory is similar to working and training on your own machine, except Google Drive is used as the default storage, and you get to use the services of an efficient GPU for free. You can save files, models parameters, etc. on your drive on regular intervals to avoid risking your data loss due to that 12 hour catch. Another cool thing about Google Colab is that, all major libraries (numpy, matplotlib, etc.) and frameworks (tensorflow, etc.) are pre-installed (just run “!pip freeze” to see the list of installed libraries and frameworks), you do not need to go through various installation processes and, instead, can immediately proceed to writing code. If any required library is missing, it can be installed with pip or apt.

So, what are you waiting for? Give it a try here.
