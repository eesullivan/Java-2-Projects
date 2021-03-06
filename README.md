# Java-2-Projects 
#### The following projects were created by James Dizikes for CS2334
#### I received full credit on each project but due to the academic nature of the code, it is hidden. However, the summation of all projects was Project 3 and my output graphs are available to view in the Project 3 folder.

All projects were about Elementary Cellular Automatons (ECA). For more information about ECAs, please visit https://mathworld.wolfram.com/ElementaryCellularAutomaton.html

## Project 1: A Simple Program with Complex Behavior
#### Overview
Given a rule number, true and false character representations, and an initial state, I created a program where the main class would do the following:
* getRuleNum(): Return the Wolfram Code for the rule that governs the evolution of the ECA.
* evolve(int numSteps): Evolve the ECA a given number of steps.
* getTotalSteps(): Return the total number of steps that the ECA has evolved. 
* getState(int stepNum): Return an array with the states of the cells after the given step. The step number
must be less than or equal to the total number of steps.
* getStateString(int stepNum): Return a String that represents the states of the cells after the given step.
The String has one character for each cell, and the symbols used to represent false and true are those
returned by getFalseSymbol() and getTrueSymbol().
* toString(): Return a String that represents the entire evolution of the ECA. The String consists of the
state String for every generation joined together by newline characters.
* save(String filename): Save the output of toString() to a file with the given name. (Overwrite the content
of the file if it already exists.)
* getFalseSymbol(): Return the character that represents false. Use ‘0’ as the default if the ECA is not
constructed from a text file.
* setFalseSymbol(char symbol): Set the character that represents false.
* getTrueSymbol(): Return the character that represents true. Use ‘1’ as the default if the ECA is not
constructed from a text file.
* setTrueSymbol(char symbol): Set the character that represents true

In order to have the above methods work, three other classes were created: Rule, Generation, and Cell.



## Project 2: Not-So-Elementary Cellular Automata
#### Overview
Project 2 builds on the ideas of Project 1. While Project 1 simulated the evolution of ECAs on a finite grid, Project 2 models ECAs using a modular design. This allows for a simulation of multiple types of rules and different boundary conditions. Project 2 also featured utility classes, AutomatonMeasurements. These calculations included the hamming distance between generations of automatons in different forms, as well as methods for calculating how many times a specific subrule is used in evolving automata generations.
For a full list of methods written, please see the Project 2 folder.



## Project 3: Visualizing Automaton Evolution
#### Overview

In Project 2, I wrote a utility class named AutomatonMeasurements (as mentioned above) to calculate quantities that describe cellular automaton evolution.
This class includes the following two methods:

1. `int[] hammingDistances(Automaton a)`: Given an Automaton that has evolved some number of steps, return an array of the Hamming distances between each successive Generation.

2. `int[][] subruleCounts(Automaton a)`: Given an Automaton that has evolved some number of steps, return an array of arrays with the number of times each subrule was used to produce each Generation. 

In this project, I used these methods along with the rest of my Project 2 code to calculate Hamming distance and subrule count data for a particular elementary cellular automaton.
Then I plotted this data using the [JavaFX] graphics library.

In the Project 3 folder, you will find my generated data plots.
