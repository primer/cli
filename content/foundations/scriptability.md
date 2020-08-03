---
title: Scriptability
---

import GhPrList from '../../images/gh-pr-list.png'
import GhPrListMachine from '../../images/gh-pr-list-machine.png'

Make choices that ensure that creating automations or scripts with GitHub commands is obvious and frictionless. Practically, this means:

- Create flags for anything interactive
- Ensure flags have clear language and defaults
- Consider what should be different for terminal vs machine output


### In terminal

<img src={GhPrList} alt="" />

### Through pipe

<img src={GhPrListMachine} alt="" />

### Differences to note in machine output:
- No color or styling
- State is explicitly written, not implied from color
- Tabs between columns instead of table layout, since `cut` uses tabs as a delimiter
- No truncation
- Exact date format
- No header
