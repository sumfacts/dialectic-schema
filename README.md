# Dialectic Schema

A specification for representing arguments in a standardized format.

> Dialectic is a discourse between two or more people holding different points of view about a subject but wishing to establish the truth through reasoned argumentation."
> -[ Wikipedia](https://en.wikipedia.org/wiki/Dialectic)

**Project status**: proof of concept

## Motivation

Today's world is a tough environment for finding out the truth about anything. Each of us has a few pieces of the puzzle and we're left to try match them up with others around us.

People in general are under time constraints and lack good tools for collaboratively debating topics. Discussions on social media are mostly noise and it is easy to skip accountability by obfuscating the truth.

What we need is a clear way of defining arguments that can then be shared, forked and collaborated upon. This will enable anybody to communicate complex ideas and ultimately demand answers to questions that dont want to be answered.

## Benefits

1. less noise - clear and simple arguments that stay purely on-topic
2. sharing - an argument can be encapsulated in a file and shared freely
4. collaboration - multiple people can asynchronously contribute to the same argument
3. versioning - arguments can be improved and refined over time
5. finding holes in arguments - see where an argument falls flat and where you are missing some pieces of the puzzle
6. exposing logical flaws more easily - ad hominems, hate-speech, confirmation bias, etc...

## Potential applications of use

- official government statements - presenting arguments for policy change
- news media - explaining current events without rhetoric and fake news
- fact-checking - analyzing arguments made by others and holding them accountable
- scientific theses - formalizing the format of academic and scientific papers
- conspiracies - legitimizing conspiracy theories and assessing their truthfulness
- knowledge sharing - over time building a body of knowledge that future generations can digest easily and learn from

## Proof of concept

```
{
  type: 'argument',
  value: 'Aliens exist',
  thesisArguments: [
    {
      type: 'argument',
      value: 'There was a crash at Roswell',
      ...
    },
    ...
  ],
  antithesisArguments: [
    {
      type: 'argument',
      value: 'There is no official evidence for aliens.',
      ...
    },
  ],
  references: [
    ...,
  ],
  author: ...,
  version: ...,
}
```
