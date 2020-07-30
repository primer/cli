---
title: Language
---

Language is the most important tool at our disposal for creating a clear, understandable product. Having clear language helps us create memorable commands that are clear in what they will do.

We generally follow this structure:

|gh|`<command>`|`<subcommand>`|[value]|[flags]|[value]|
|---|---|---|---|---|---|
|gh |issue|view|234|--web|-|
|gh|pr|create|-|--title|“Title”|
|gh|repo|fork|cli/cli|--clone|false|
|gh|pr|status|-|-|-|
|gh|issue|list|-|--state|closed|
|gh|pr|review|234|--approve|-|


**Command:** The object you want to interact with

**Subcommand:** The action you want to take on that object. Most gh commands contain a command and subcommand. These may take arguments, such as issue/PR numbers, URLs, file names, OWNER/REPO, etc.

**Flag:** A way to modify the command, also may be called “options”. You can use multiple flags. Flags can take values, but don’t always. Flags always have a long version with two dashes (--state) but often also have a shortcut with one dash and one letter (-s). It’s possible to chain shorthand flags: -sfv is the same as -s -f -v

**Values:** Are passed to the commands or flags
- The most common command values are:
  - Issue or PR number
  - The “owner/repo” pair
  - URLs
  - Branch names
  - File names
- The possible flag values depend on the flag:
  - `--state` takes `{closed | open | merged}`
  - `--clone` is a boolean flag
  - `--title` takes a string
  - `--limit` takes an integer


Tip: To get a better sense of what feels right, try writing out the commands in the CLI a few different ways.

 DO. 							 DO NOT.
gh pr review --approve			gh pr approve

Approve is a type of review, so we use a flag instead of a command here.


When designing your command’s language system:
- Use GitHubby language
- Use unambiguous language that can’t be confused for something else
open vs create
- Use shorter phrases if you can
  - pr vs pull request
  - repo vs repository

 DO. 							 DO NOT.
gh pr create					gh pr open

 DO. 							 DO NOT.
gh repo view					gh repository view
