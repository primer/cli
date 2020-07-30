---
title: Scriptability
---

Make choices that ensure that creating automations or scripts with GitHub commands is obvious and frictionless. Practically, this means:

- Create flags for anything interactive
- Ensure flags have clear language and defaults
- Consider what should be different for terminal vs machine output



In terminal (gh issue list)

```
Showing 30 of 229 issues in cli/cli

#1360  Ability to skip confirmation via a flag                                         about 20 minutes ago
#1358  Provide extra options for merge conflicts      (enhancement)                    about 1 day ago
#1354  Add ability to manage user's all repos fro...  (enhancement, needs-user-input)  about 1 day ago
#1353  Listing releases and assets                    (enhancement)                    about 3 days ago
#1349  Ability to edit title/body of already open PR  (enhancement)                    about 3 days ago
```

Through pipe (gh issue list | cat)

```
1360    Ability to skip confirmation via a flag         2020-07-14 16:58:27 +0000 UTC    OPEN
1358    Provide extra options for merge conflicts       enhancement     2020-07-13 04:14:14 +0000 UTC    OPEN
1354    Add ability to manage user's all repos from CLI needs-user-input   2020-07-13 14:52:36 +0000 UTC    OPEN
1353    Listing releases and assets     enhancement     2020-07-11 04:55:06 +0000 UTC    OPEN
1349    Ability to edit title/body of already open PR   enhancement     2020-07-11 15:21:00 +0000 UTC    OPEN
```

Differences to note in machine output:
- No color or styling
- State is explicitly written, not implied from color
- Tabs between columns instead of table layout
- The “cut” command uses tabs as a delimiter
- No truncation
- Exact date format
- No header
