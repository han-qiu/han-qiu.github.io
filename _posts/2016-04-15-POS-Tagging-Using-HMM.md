---
layout: post
title: "POS-Tagging Using trigram HMM with viterbi algorithm"
publish: true
---

### Hidden-Markov Model

In this task, I preformed a 3-gram Hidden-Markov Model to do some Chinese POS-Tagging.
The codes are written in python,you can type in the command line:

> python hmm.py

to run it.(This pretty slow, about 10 minutes on my laptop)

### The functions and structure

![code]({{site.url}}/images/hmm.png)

### Something about my Model

At first, I performed a pure HMM, the correctness is very low:25.6%

Later I found that there are lots of words in the dev set doesn't occur in the training set. So the emission probability is 0, which make the tagging of whole sentence goes wrong

Then I did some statistics, and found out that:
> 781 words in the developing set are not in the training set
> 67 trigrams in the developing set are not included in the training set
> 2 bigrams in the developing set are not included in the training set

After I did a naive trick:

> set the emission probability to 10^-5 if it's 0

my model got the correctness of 89.26%

And after I add back-off(just to bigram)

the correctness is 89.39%

### What cam be improved

1. maybe back-off to unigram ?(I didn't do this because back-off to bigram just increased my model a tiny bit)

2. some tuning, because my algorithm is very slow, so I didn't do much thing to tune the parameter, I suppose that may helps.

### What I learned from this assignment
**You cann't write bug-free codes, so it's very very very important to test**

1. Unit test: every time you write a module, you must perform unit test, or it will be
very difficult to debug

2. test your algorithm with a small data set(e.g:one sentence in this assignment),
**Especially after you changed your algorithm**, or you may waste your time to run the code and find it that it's totally wrong.
