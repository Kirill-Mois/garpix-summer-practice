# garpix-summer-practice

## Task
A list of loads and their attributes is given: size, the ability to rotate them, the ability to put another load on them, and others. Also, several cargo spaces are given along with an algorithm that takes a list of cargo spaces and a corresponding cargo group for each cargo space, and calculates the amount of unfilled space after the cargo is stowed. The task is to sort the general list of loads into groups for stowing in each cargo space, so that after calculating the algorithm, the amount of unfilled space is minimal.

## Algorithm

1. Calculate the number of a given cargo spaces, enough for stowing all the given loads.
2. For each of the cargo spaces, create two types of groups of leads for stowing: one for the random algorithm, one for the optimized algorithm.
3. Sort the list of loads by their volume and attributes.
4. Add loads into the groups:
	Random algorithm:
	- on iteration, add one random load into each group
	Optimized algorithm:
	- on even iteration, add the first load from the sorted list into each group from the first to the last
	- on odd iteration, add the first load from the sorted list into each group from the last to the first
5. Start calculation of unfilled space with random groups and optimized groups
6. Compare the results
