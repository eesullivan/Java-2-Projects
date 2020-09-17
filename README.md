# Java-2-Projects 
#### The following projects were created by James Dizikes for CS2334
#### I received full credit on each project


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




## Project 3: Visualizing Automaton Evolution
#### Overview

In Project 2, I wrote a utility class named `AutomatonMeasurements` to calculate quantities that describe cellular automaton evolution.
This class includes the following two methods:

1. `int[] hammingDistances(Automaton a)`: Given an Automaton that has evolved some number of steps, return an array of the Hamming distances between each successive Generation.(The length of the array is equal to the number of steps.)

2. `int[][] subruleCounts(Automaton a)`: Given an Automaton that has evolved some number of steps, return an array of arrays with the number of times each subrule was used to produce each Generation. 
(The length of the array is equal to the number of steps, and the length of each subarray is equal to the number of subrules.)

In this project, I used these methods along with the rest of my Project 2 code to calculate Hamming distance and subrule count data for a particular elementary cellular automaton.
Then I plotted this data using the [JavaFX] graphics library.

In the Project 3 folder, you will find my generated data plots.
