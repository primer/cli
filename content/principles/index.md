---
title: Principles
---

import {DoDontContainer, Do, Dont, Caption} from '@primer/gatsby-theme-doctocat'
import {Box, Flex, BorderBox, Text, CircleOcticon} from '@primer/components'
import {CheckIcon} from '@primer/octicons-react'
import {XIcon} from '@primer/octicons-react'
import Principle201 from '../../src/images/Principle2-01.png'
import Principle202 from '../../src/images/Principle2-02.png'
import Principle204 from '../../src/images/Principle2-04.png'
import Principle205 from '../../src/images/Principle2-05.png'
import Principle401 from '../../src/images/Principle4-01.png'
import Principle402 from '../../src/images/Principle4-02.png'
import Principle403 from '../../src/images/Principle4-03.png'

## Reasonable defaults, easy overrides
Optimize for what most people will need to do most of the time, but make it easy for people to adjust it to their needs.

## Make it feel like GitHub
Using this tool, it should be obvious that it’s GitHub and not anything else. Use details that are specific to GitHub, such as language or color. When designing output, reflect the GitHub.com interface as much as possible and appropriate.


<DoDontContainer>
  <Do src={Principle205}>
    Use language accurate to GitHub.com
  </Do>
  <Dont src={Principle202}>
    Don't use language that GitHub.com doesn't use
  </Dont>
</DoDontContainer>

<DoDontContainer>
  <Do src={Principle204}>
    Use sentence case
  </Do>
  <Dont src={Principle201}>
    Don't use title case
  </Dont>
</DoDontContainer>

**Resources**
- [GitHub Brand Content Guide](https://brand.github.com/content/)


## Reduce cognitive load
Command line interfaces have very few affordances, rely on memory, and are often unforgiving of mistakes. We do our best to design our commands to mitigate this.

Reducing cognitive load is necessary for  [making an accessible product](https://www.w3.org/TR/coga-usable/#summary) .

**Ways to reduce cognitive load**
* Include confirm steps, especially for riskier commands
* Include headers to help set context for output
* Ensure consistent command language to make memorizing easier
* Ensure similar commands are visually and behaviorally parallel.
	* For example, any create command should behave the same
* Anticipate what people might want to do next.
	* For example, we ask if you want to delete your branch after you merge.
* Anticipate what mistakes people might make


## Bias towards terminal, but make it easy to get to the browser
We want to keep people in the terminal wherever we can to maintain focus and reduce context switching, but when it’s necessary to jump to GitHub.com make it obvious, fast, and easy. Certain actions are probably better to do in a visual interface.

Examples
* —web flags
* outputting URLs
* Preview in browser step


<img src={Principle401} alt="" />
<Caption>A beautiful husky puppy.</Caption>

<img src={Principle402} alt="" />


<img src={Principle403} alt="" />
