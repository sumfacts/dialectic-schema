# Dialectic Schema

A specification for representing arguments in a standardized format.

> Dialectic is a method of examining and discussing opposing ideas in order to find the truth."
> -[ Merriam-Webster Dictionary](https://www.merriam-webster.com/dictionary/dialectic)

**Project status**: [proof of concept](https://github.com/sumfacts/dialectic-schema/issues/1)

## Motivation

Today's world is a tough environment for finding out the truth about anything. Each of us have a few pieces of the puzzle and we're left to try match them up with others around us.

People in general are under time constraints and lack good tools for collaboratively debating topics. Discussions on social media are mostly noise and it is easy to skip accountability by obfuscating the truth.

What we need is a clear way of defining arguments that can then be shared, forked and collaborated upon. This will enable anybody to communicate complex ideas and ultimately demand answers to questions that dont want to be answered.

## Benefits

1. less noise - clear and simple arguments that stay purely on-topic
2. shareable - an argument can be encapsulated in a file and shared freely
4. collaboration - multiple people can asynchronously contribute to the same argument
3. versioning - arguments can be improved and refined over time using version control
5. find holes in arguments - see where an argument falls flat and where you are missing some pieces of the puzzle
6. expose logical flaws more easily - ad hominems, hate-speech, confirmation bias, etc...

## Potential applications of use

- official government statements - presenting arguments for policy change
- news media - backing up claims made in reports with solid arguments and evidence. It will make it easier to weed out fake news sources
- fact-checking - analyzing arguments made by others and holding them accountable
- scientific theses - formalizing the format of academic and scientific papers
- conspiracies - legitimizing theories and assessing their truthfulness
- knowledge sharing - over time building a body of knowledge that future generations can digest easily and learn from
- legal - cases can be built and put forward in a standardized way

## Example

```
{
  argument: 'Aliens exist',
  supportingArguments: [
    {
      argument: 'There was a crash at Roswell',
      ...
    },
    ...
  ],
  opposingArguments: [
    {
      argument: 'There is no official evidence for aliens.',
      ...
    },
  ],
  references: [
    ...,
  ],
  author: ...,
  version: ...,
  ...
}
```
