# Shortest Path
## About
Shortest path algorithims help a computer determine what the shortest path between two nodes are in a graph. And the distance of this path. In this project I have implemented both the [dijkstra's algorithim](https://en.wikipedia.org/wiki/Dijkstra's_algorithm) and the [A* algorithim](https://en.wikipedia.org/wiki/A*_search_algorithm).
## Installation
In order to run and test this code for yourself first clone the repo:
```Bash
$ git clone https://github.com/koochi10/Shortest-Path.git
$ cd Shortest-Path/
```
In order to compile the code run:
```Bash
$ make
```
With this code we are able to use both algorithms and anaylze the run time complexity of both of them. We are gonna test both of the algorithims from a graph of San Fransisco. Before we get started it is important to note that the files containing the graph have been preprocessed to fit the input for both dijkstra and A* algorithims. 

To test dijkstra's algorithim we run:
```Bash
$ ./path dijkstra SF.cedge 0 2
```
where 0 and 2 represent some arbitrary nodes in the graph.

To test A* algorithim we run:
```Bash
$ ./path Astar SF.cedge SF.cnode 0 2
```
As we can see, we must include an extra file as input for this function. This is because the A* algorithim utlizes the x and y coordinates of nodes as well as an edge list to optimize its runtime.
