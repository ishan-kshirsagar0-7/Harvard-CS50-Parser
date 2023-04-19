# Harvard CS50 AI (Week 6) Project 11 : Parser

This is the eleventh project of [Harvard CS50's Introduction to Artificial Intelligence course](https://cs50.harvard.edu/ai/2020/), the first project of Week 6.

## My Outputs

![Screenshot of my output on terminal](https://cdn.discordapp.com/attachments/1091358303063396496/1098332149939187712/image.png)

## Objective

Write an AI to parse sentences and extract noun phrases.

## Background

A common task in natural language processing is parsing, the process of determining the structure of a sentence. This is useful for a number of reasons: knowing the structure of a sentence can help a computer to better understand the meaning of the sentence, and it can also help the computer extract information out of a sentence. In particular, it’s often useful to extract noun phrases out of a sentence to get an understanding for what the sentence is about.

In this problem, we’ll use the context-free grammar formalism to parse English sentences to determine their structure. Recall that in a context-free grammar, we repeatedly apply rewriting rules to transform symbols into other symbols. The objective is to start with a nonterminal symbol S (representing a sentence) and repeatedly apply context-free grammar rules until we generate a complete sentence of terminal symbols (i.e., words). The rule S -> N V, for example, means that the S symbol can be rewritten as N V (a noun followed by a verb). If we also have the rule N -> "Holmes" and the rule V -> "sat", we can generate the complete sentence "Holmes sat.".
