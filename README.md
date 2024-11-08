# Graph Representations

Implement a function that converts an adjacency matrix to an adjacency list for
a directed unweighted graph using the template in `code.js`. Test your new
function; I've provided some basic testing code that uses
[jsverify](https://jsverify.github.io/) in `code.test.js`. Now, the test code
does contain the solution, so you can have a look at it if you get stuck, but
try not to peek before attempting to solve it on your own.

## Runtime Analysis

What is the runtime complexity of the conversion that you implemented? Does it
depend on the number of vertices, the number of edges, or both?

Describe your reasoning and the conclusion you've come to. Your reasoning is the
most important part. Add your answer to this markdown file.

## Bonus

Implement a function to convert an adjacency list to an adjacency matrix and
analyze it as above.

## Runtime Analysis, Maxie M.

**Vertices (V)**
- Will be the number of rows (or columns) in the adjacency matrix

**Edges (E)** 
- Will be the number of 1’s in the matrix 

**Worst Case** 
- The worst case would occur when there is a fully connected graph 
- If this happens, the adjacency matrix has $V^2$ elements to check 
- $\text{Time Complexity} = O(V^2)$
- Complexity depends on the number of vertices when checking each potential connection. This happens regardless of the presence of an edge or not.

**Conclusion** 
- $\text{Runtime Complexity} = O(V^2)$
  - Due to having to traverse every cell in the $V \times V$ adjacency matrix
- This complexity will hold regardless of the amount of edges present
  - Due to checking each cell individually for the presences of an edge 

## Plagiarism Statement: 
I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.

## Resources: 
- https://www.geeksforgeeks.org/graph-and-its-representations/
