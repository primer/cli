---
title: Syntax
---

import {DoDontContainer, Do, Dont, Caption} from '@primer/gatsby-theme-doctocat'
import SyntaxBranch from '../../images/Syntax-Branch.png'
import SyntaxLabel from '../../images/Syntax-Label.png'
import SyntaxRepo from '../../images/Syntax-Repo.png'

## Branches
Display branch names in brackets and/or cyan

<img src={SyntaxBranch} alt="" />

## Labels
Display labels in parenthesis and/or gray

<img src={SyntaxLabel} alt="" />

## Repository
Display repository names in bold where appropriate

<img src={SyntaxRepo} alt="" />


## Help
Use this consistent language in docs to explain command usage.

https://github.com/cli/cli/blob/trunk/docs/command-line-syntax.md

### Literal text

Use plain text for parts of the command that cannot be changed

```
gh help
```

<Caption>The argument help is required in this command</Caption>

### Placeholder values

Use angled brackets to represent a value the user must replace. No other expressions can be contained within the angled brackets.

```
gh pr view <issue-number>
```

<Caption>Replace "issue-number" with an issue number</Caption>

### Optional arguments

Place optional arguments in square brackets. Mutually exclusive arguments can be included inside square brackets if they are separated with vertical bars.


```
gh pr checkout [--web]
```

<Caption>The argument `--web` is optional.</Caption>

```
gh pr view [<number> | <url>]
```

<Caption>The "number" and "url" arguments are optional.</Caption>

### Required mutually exclusive arguments

Place required mutually exclusive arguments inside braces, separate arguments with vertical bars.

```
gh pr {view | create}
```

### Repeatable arguments

Ellipsis represent arguments that can appear multiple times

```
gh pr close <pr-number>...
```

### Variable naming

For multi-word variables use dash-case (all lower case with words separated by dashes)


```
gh pr checkout <issue-number>
```

### Additional examples

Optional argument with placeholder:
```
command subcommand [<arg>]
```

Required argument with mutually exclusive options:
```
command subcommand {<path> | <string> | literal}
```

Optional argument with mutually exclusive options:
```
command subcommand [<path> | <string>]
```
