# Contributing to DOME

Thank you for your interest in contributing to the DOME project. It means so much to us.
These are the guidelines you should follow to contribute to DOME. Please use your best judgement.

## Code of Conduct

This project is released with a Contributor [Code of Conduct](https://github.com/avivbeeri/dome/blob/master/CODE_OF_CONDUCT.md). 
By participating in this project you agree to abide by its terms.

## How can I contribute?

### Reporting a Bug / Suggesting an Enhancement

If you find a bug, or want to suggest a new feature or piece of functionality, simply raise an issue and we will consider it.

### Submitting a Pull Request

To submit a pull request, you should fork the repository and create a new branch for your feature. You can then push this back to GitHub and open a Pull Request in the DOME repository.

## Where can I ask for help?

You can ask for help working on DOME in [our Discord server](https://github.com/avivbeeri/dome), or raise an issue asking for help.

## Design Philosophy

DOME is designed and implemented according to a set of core principles:

Minimalism: DOME is a minimal, but all-in-one toolkit. This means that it should only contain things a majority of projects would benefit from. Almost everything is introduced into the core engine with a specific use-case in mind. It's preferred to implement new features as libraries "on-top" of DOME, rather than including everything in the core. The libraries which are frequently moved from project to project make good candidates for new features.

Usage-First: Any new API is designed "usage-first", and then an implementation is built around that. This allows for a more "comfortable" and developer-friendly API, because it's how we would _want_ to use it. Once the API is designed, we do what we can to build an implementation to fit that design, adjusting when technical reasons require it.


## Coding Conventions and Style Guides

Code won't be merged into DOME if it doesn't match the existing code style. Here are some of the more obvious style decisions in the codebase.

### C Style

C-code should conform to the following:

* Variables are named with camelCase.
* Functions are named with camelCase.
* Structs which represent "objects" are usually declared in all capitals.
* Methods associated with structs are named with the format `NAME_methodName()`
* Braces are required for control-flow blocks: `while`, `for` and `if` must be followed by a `{` and `}` to mark out the statements which are predicated on that control flow. This is to prevent copy-paste errors, as well as poor semi-colon placement.
```
if (condition) { // This brace is on the same line as the ending parenthesis.
  ...
}
```

* A space must be placed after these keywords, and before parenthesis of their conditions.
```
while (condition) {
  ...
}
```

### Wren

Wren code should conform to the following:

* Classes are named with TitleCase, each word being capitalised, including the first.
* Variables, methods and properties all require camelCase, unless they are intended to be constants, in which case they should be fully uppercase with underscore seperation between words.
```
var DEGREE_OF_SEPERATION = 6

class GraphVisitor {
  static newProperty { _property }
  static MAX_TRIES { 4 }
  static someMethod(withInput) { ... }
}
```
* Spaces around control-flow constructs, in similarity to C-styles.
* Braces around control-flow blocks.

## Contributors

People who have contributed code or documentation to the project:
* Aviv Beeri, aka springogeek [https://github.com/avivbeeri]
* scholar-mage [https://github.com/scholar-mage]
* Francisco Requena, aka frarees [https://github.com/frarees]
* Camilo Castro, aka clsource [https://github.com/clsource]
