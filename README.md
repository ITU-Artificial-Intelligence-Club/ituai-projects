# ITU Artificial Intelligence Club Projects

This repository is made to keep track of the current projects of ITU AI Club.

All the current and upcoming projects are listed in the [projects](projects) folder with their descriptions, specificaions and requirements. People who are currently working on the projects are also listed in the project files.


## Projects

### Upcoming

| Title               | Languages           | Reviewers        | Accepting Contributors |
|---------------------|---------------------|------------------|------------------------|
| CezRoom             | TypeScript & Python | Utku Biçer       | Yes                    |
| ITUGuessr           | TypeScript & Python | Ertuğrul Şentürk | Yes                    |
| Mailo               | Python              | Utku Biçer       | Yes                    |
| Reverse Turing Test | TypeScript          | Ertuğrul Şentürk | Yes                    |


### Current

There are no current projects, for now...


## Contributing Conventions & Guidelines

If you want to work on the projects, there are some conventions and guidelines that you should follow.


### General Communication

For most parts, communication through GitHub will be in English. If you lack the ability to express yourself in some parts, Turkish is acceptable. Yet for writing code, documentation, issues, PRs and comments; it is desired to use English.

This is mainly because:
- There may be people who do not speak Turkish
- Most of the jargon in programming is in English
- In the field, you will need to use English in most cases


### Git & GitHub Usage

All the projects will be managed through GitHub, obeying the following rules:

**Branches**: Origin branch is `main`.

For the branch names, use the following pattern: `type/description`. For example, `feature/login`, `fix/bug-in-register` or `docs/update-readme`.

**Commits**: We are using conventional commits. For more information, check [this site](https://www.conventionalcommits.org/en/v1.0.0/).

Basically, the commit message should be like this: `<type>[optional scope]: <description>`

For example:

`feat: add encryption to passwords in the database`
`feat[backend]: add selection of characters to the chat`
`refactor: change the way the user is authenticated`
`docs: update the README.md to include the new features`

Generaly used types: `feat`, `fix`, `docs`, `style`, `refactor`, `test`, `chore`

There is need to be too explanatory, but the commit message should be clear and concise. Your colleagues should understand what you did by reading the commit message.

**Pull Requests**: The PRs should have a title and a description, explaining what was done and why.

If there is an issue related to the PR, you should link the issue in the PR description.

Try to be as clear and explanatory as possible in the PR description. Even if there is a small change, mentioning it will help your colleagues review your PR faster & easier.


### Languages & Syntax

**Python Syntax**: We are using PEP8 for the Python syntax. For more information, check [this site](https://peps.python.org/pep-0008/).

Basically we will use:
- camelCase for functions 
- snake_case for variables
- UpperCamelCase for classes
- UPPER_CASE for constants
- 2 spaces for indentation

Other language conventions will be added here in the future.


### Documentation

**Code Documentation**: There is no certain rule for writing in-code documentation, but try to be as clear as possible. For function, methods, classes and scripts, try to write at least a small description of what it does.

**General Documentation**: In general, when you are documenting your work, how-to or setup guides etc, create a new markdown file in the `docs` directory of the project. If there is no `docs` directory, create one. It is essential that we use markdown format.
