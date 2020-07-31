---
title: Process
---


When designing a new feature, consider:

1. **What the command does**
	1. What makes sense to do from a terminal? What doesn’t?
	2. What might people want to automate?
	3. What is the default behavior? What flags might you need to change that behavior?
	4. What might people try and fail to do and how can you anticipate that?
2. **What the command is called**
	1. What should the  [command language system](/foundations/language)  be?
	2. What should be a command vs a flag?
	3. How can you align the language of the new command with the existing commands?
3. **What the command outputs**
	1. What can you do to make the CLI version [feel like the GitHub.com version](/principles#make-it-feel-like-github), using [color](/foundations/color), [language](/foundations/language), [spacing](/foundations/spacing), info shown, etc?
	2. How should the [machine output](/foundations/scriptability) differ from the interactive behavior?
4. **How you explain your command**
	1. You will need to provide a short and long description of the command for the [help pages](/components/help).
5. **How people discover your command**
	1. Are there ways to integrate CLI into the feature where it exists on other platforms?
