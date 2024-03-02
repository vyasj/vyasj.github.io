---
layout: page
title: markov chain sentence generator
description: a program that reads text and generates a markov chain to then produce its own sentences given a prompt word
img: assets/img/markovchain.png
importance: 1
category: work
related_publications: true
---

The primary driver behind starting this project was the desire to get better at writing code in Rust. I'm by no means a good programmer, but the goal is to get my code from Absolutely Terrible to Slightly Less Terrible. 

I've actually implemented something like this before for a college class, though it was in C++. Still, I was able to use the same ideas to write this one, and even though I haven't built the full functionalities I had in mind yet, it does indeed generate sentences. Here's an example:

Command: 
    load beemovie.txt 15
    generate most_common honey 10

Output: 
    `honey and gentlemen of the honey and gentlemen of the honey`

As you can see, it's not the greatest at generating valid sentences, despite this command being run with a context depth of 15 words. I think I may have to debug by printing the markov chain and seeing what the frequencies actually are, to then determine if it really is an issue with the code or just the input text file. 

After that, I would want to implement random sentence generation as well, where you just give it a starting word, and it will randomly pick from the previously seen following words and generate a sentence of given length. For now though, this is funny enough. I may revisit this sometime in the future, and edit this page.

The code can be found <a href="https://github.com/vyasj/markov">here</a>.