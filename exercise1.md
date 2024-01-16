# Exercise 1

## Language & Framework

For this exercise, I decided to choose Haskell. Haskell is a general-purpose, purely functional programming language with a steadily growing ecosystem.

### Building

Unlike Python or JS, Haskell is a compiled language, so an explicit build step is required. GHC, the Glasgow Haskell Compiler, can be used to compile Haskell modules into executable files. In addition to GHC, there are two popular build systems: Cabal and Stack. Stack is the more modern of the two, and it simplifies initializing, building, and testing Haskell projects, as well as managing project dependencies.

### Linting

Haskell also has dedicated utilities for linting and code formatting. HLint is a popular linting tool, with rich code editor and IDE support. HLint is also included in haskell-language-server (HLS). Another tool is stylish-haskell, a simple code prettifier with HLS support.

### Testing

There are also quite a few testing libraries in Haskell. QuickCheck is a popular library for property-based testing. Another popular testing library is HUnit, which, as the name suggests, is used for unit testing.

## CI/CD Tools

Besides Jenkins and GitHub Actions, there are a multitude of tools, both self-hosted and cloud-based, that offer similar functionality. To keep this text short, we will only list some of the most widely used ones. GitLab, a code-sharing platform similar to GitHub, offers their own cloud-based CI/CD tool. TeamCity is a CI/CD tool developed by JetBrains, which can either be set up on the cloud or be hosted on-premises. Finally, Atlassian Bamboo is a cloud-based CI/CD program that provides seamless integration with Jira and BitBucket.

## Self-hosted vs. Cloud-based

I think that a self-hosted environment would be better for this project. Haskell isn't quite as popular as other mainstream languages, so setting up the environment would be problematic in many cloud-based solutions. In contrast, setting up the environment and installing the necessary tools can be done more easily in a self-hosted environment, since we have a complete control over our CI/CD server. This task can further be simplified, because Haskell has support for Docker.

It must be noted that the above problem does not apply to GitHub Actions. A quick search on the GitHub Marketplace shows that there are third-party actions to set up Haskell environment. Issues could arise if the team wanted to use a different cloud-based tool, though.

In general, there are many factors to consider when choosing an appropriate environment, such as the complexity of the software project and the size and structure of the company.
