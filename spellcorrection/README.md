# spellcorrection

## Description
In this project, I have developed an algorithm which utilizes Bayesian inference to correct spelling errors.

# How It Works: Probability Theory
The call corrected-word(w) tries to choose the most likely spelling correction for w. There is no way to know for sure (for example, should "lates" be corrected to "late" or "latest" or "lattes" or ...?), which suggests we use probabilities. We are trying to find the correction c, out of all possible candidate corrections, that maximizes the probability that c is the intended correction, given the original word w:

## Output 
>>> corrected-word('speling')
'spelling'



## Installation

  $ java -jar spellcorrection-0.1.0-standalone.jar [args]



## Usage

This code is used in the Electronic Health Record system of hospitals to auto correct the spelling and for auto-suggestion.
When a healthcare professional type more than  characters, this algorithm suggest them words that are frequently used in healthcare domain. 

## Limitation

Using Bayesian approach, there was a limitation where top suggested words were not the required word by health professional of particular department.

## Solution
To solve above limition 60% weighatge was given to the word that comes from baysian inference and 40% weightage was given to the word that was used/selected by professionals earlier while using the EMR platform.



