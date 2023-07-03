# Polygon-Genetic-Algorithm
## Introduction
The code is an implementation of a genetic algorithm for solving a specific problem related to polygon generation and analysis. Let's go through the code, explain its structure and flow, and add some notes along the way.

![image](https://github.com/HammadHk1/Polygon-Genetic-Algorithm/assets/117303560/c9e3f79b-d996-47d3-88bb-1e779b675fc8)

## Flow of Code:
- The code consists of three classes: `Shape`, `Binary`, and `Genetic_Algorithm`. Let's discuss each class in more detail:

- Shape: This class represents a shape and contains methods related to drawing the shape and generating random axis coordinates. The constructor takes a parameter Plane, which is used as the size for drawing the polygon. The Draw method uses the Axis coordinates to draw the shape using the plt.plot function from matplotlib. The Generate_Random_Axis method generates random axis coordinates within the specified Plane size.

- Binary: This class is not used in the provided code. It seems to be intended for binary number conversion, but it is incomplete and not utilized anywhere.

- Genetic_Algorithm: This class contains methods for performing genetic algorithm operations for polygon generation and analysis. It has various functions for chromosome manipulation, crossover, mutation, fitness evaluation, and other related operations. The Make_Chromosomes method takes a list of axis coordinates and converts them into a chromosome representation. The `CrossProduct` method calculates the cross product of two vectors. The `isConvex` method checks if a polygon formed by given points is convex. The Check_Intersection method checks if the polygon represented by a chromosome has any self-intersections using the Shapely library. The CrossOver method performs crossover between two chromosomes. The Mutation method is incomplete and does not have any functionality. The `Fitness_Function` method calculates the fitness value of a chromosome based on convexity and intersection checks. The Get_Chromosomes and `Get_CC` methods return the chromosomes and children chromosomes, respectively. The Get_Fitness method returns the fitness values of all chromosomes, sorted in ascending order.

- The code then creates instances of the `Shape` and `Genetic_Algorithm` classes, generates random axis coordinates using Generate_Random_Axis, and passes them to the Fitness_Function method to evaluate their fitness values. The fitness values are stored in the Fitness_Value dictionary. The Get_Fitness method sorts the fitness values and returns them.

- Next, the code performs the crossover operation by calling the `CrossOver` method on pairs of chromosomes. This operation creates new chromosomes based on the crossover of existing ones. The resulting chromosomes are stored in the Chromosomes list.

- Finally, the code prints the chromosomes resulting from the crossover operation and their count. It then selects the chromosome with the lowest fitness value (assuming the fitness values are sorted) and uses its axis coordinates to draw the shape using the Draw method from the Shape class.

## Note
It's important to note that the code has a few issues and incomplete parts. The Binary class is not used and seems unfinished. The Mutation method in the Genetic_Algorithm class is empty and does not perform any mutation. Additionally, there are some missing imports (random, plt, shapely) that are necessary for the code to run properly.

## Resources
- Download VScode  from below link
```
[https://visualstudio.microsoft.com/downloads/](https://code.visualstudio.com/download)
```
