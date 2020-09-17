# Java-2-Projects (from CS2334, James Dizikes)

# Project 1

# Project 2

# Project 3: Visualizing Automaton Evolution
## Overview

In Project 2, I wrote a utility class named `AutomatonMeasurements` to calculate quantities that describe cellular automaton evolution.
This class includes the following two methods:

1. `int[] hammingDistances(Automaton a)`: Given an Automaton that has evolved some number of steps, return an array of the Hamming distances between each successive Generation.(The length of the array is equal to the number of steps.)

2. `int[][] subruleCounts(Automaton a)`: Given an Automaton that has evolved some number of steps, return an array of arrays with the number of times each subrule was used to produce each Generation. 
(The length of the array is equal to the number of steps, and the length of each subarray is equal to the number of subrules.)

In this project, I used these methods along with the rest of my Project 2 code to calculate Hamming distance and subrule count data for a particular elementary cellular automaton.
Then I plotted this data using the [JavaFX] graphics library.

In the Project 3 folder, you will find my generated data plots.
