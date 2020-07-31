---
title: Spacing
---

import {DoDontContainer, Do, Dont, Caption} from '@primer/gatsby-theme-doctocat'
import GhPrList from '../../src/images/gh-pr-list.png'
import GhPrStatus from '../../src/images/gh-pr-status.png'
import GhPrStatusCompressed from '../../src/images/gh-pr-status-compressed.png'

You can use the following to create hierarchy and visual rhythm:

- Line breaks
- Tables
- Indentation


<DoDontContainer stacked>
  <Do src={GhPrStatus}>
    Use space to create more legible output
  </Do>
  <Dont src={GhPrStatusCompressed}>
    Not using space makes output difficult to parse
  </Dont>
</DoDontContainer>
