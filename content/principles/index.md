---
title: Principles
---

import {Box, Flex, BorderBox, Text, CircleOcticon} from '@primer/components'
import {Check} from '@primer/octicons-react'
import {X} from '@primer/octicons-react'
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


<Flex flexDirection={['column', 'row', 'row']}>
  <Box mr="2"  mb="4">
    <Flex flexDirection="row" alignItems="center" mb="2">
      <CircleOcticon icon={Check} size={16} bg="green.5" color="white" mr="2" p="1"/>
      <Text fontWeight="bold" color="gray.9" ml="1">
        Do
      </Text>
    </Flex>
    <Box>
      <img src={Principle204} width="50%" />
    </Box>
    <Text fontSize="0" color="gray.5">
      Use brief and direct communication
    </Text>
  </Box>
  <Box mr="2">
    <Flex flexDirection="row" alignItems="center" mb="2">
      <CircleOcticon icon={X} size={16} bg="red.5" color="white" mr="2" p="1"/>
      <Text fontWeight="bold" color="gray.9" ml="1">
        Don't
      </Text>
    </Flex>
    <Box borderRadius="3">
      <img src={Principle201} width="50%" />
    </Box>
    <Text fontSize="0" color="gray.5">
      Don't use wordy and redundant copy
    </Text>
  </Box>
</Flex>

<Flex flexDirection={['column', 'row', 'row']}>
  <Box mr="2"  mb="4">
    <Flex flexDirection="row" alignItems="center" mb="2">
      <CircleOcticon icon={Check} size={16} bg="green.5" color="white" mr="2" p="1"/>
      <Text fontWeight="bold" color="gray.9" ml="1">
        Do
      </Text>
    </Flex>
    <Box>
      <img src={Principle205} width="50%" />
    </Box>
    <Text fontSize="0" color="gray.5">
      Use brief and direct communication
    </Text>
  </Box>
  <Box mr="2">
    <Flex flexDirection="row" alignItems="center" mb="2">
      <CircleOcticon icon={X} size={16} bg="red.5" color="white" mr="2" p="1"/>
      <Text fontWeight="bold" color="gray.9" ml="1">
        Don't
      </Text>
    </Flex>
    <Box borderRadius="3">
      <img src={Principle202} width="50%" />
    </Box>
    <Text fontSize="0" color="gray.5">
      Don't use wordy and redundant copy
    </Text>
  </Box>
</Flex>

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
<Text textAlign="center" fontSize="1" color="gray.6">
  Enable and disable libraries of components from across your team.
</Text>

<img src={Principle402} alt="" />


<img src={Principle403} alt="" />
