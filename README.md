# Dialectic Schema

A specification for representing arguments in a standardized format.

> Dialectic is a discourse between two or more people holding different points of view about a subject but wishing to establish the truth through reasoned argumentation."
> -[ Wikipedia](https://en.wikipedia.org/wiki/Dialectic)

## Motivation

Today's world is a tough environment for finding out the truth about anything. No one has a complete picture and we are left putting the jigsaw puzzle together in the dark.

People in general are under time constraints and lack good tools for collaboratively debating topics. Discussions on social media are mostly noise and it is easy to skip accountability by obfuscating the truth.

What we need is a clear way of defining arguments that can then be shared, forked and collaborated upon. This will enable anybody to communicate complex ideas and ultimately demand answers to questions that dont want to be answered.

## Proof of concept

```
{
  type: 'argument',
  value: 'Aliens exist',
  author: ...,
  version: ...,
  updatedAt: ...,
  thesis: [
    {
      type: 'argument',
      value: 'There was a crash at Roswell',
      weight: 0.4,
      ...
    },
    ...
  ],
  antithesis: [
    {
      type: 'argument',
      value: 'There is no official evidence for aliens.',
      weight: 0.9,
      ...
    },
  ],
  tokenizedValue: [
    { type: 'subject', value: 'alien', plural: true, ... },
    { type: 'action', value: 'exist', ... },
  ],
  references: [
    ...,
  ],
  synthesis: ...,
}
```
