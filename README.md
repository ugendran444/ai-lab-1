

# Ex.No: 1  Implementation of Breadth First Search
### DATE: 12.08.2025                                                                          
### REGISTER NUMBER : 212222060283
### AIM: 
To write a python program to implement Breadth first Search. 
### Algorithm:
1. Start the program
2. Create the graph by using adjacency list representation
3. Define a function dfs and take the set “visited” is empty 
4. Search start with initial node. Check the node is not visited then print the node.
5. For each neighbor node, recursively invoke the bfs search.
6. Call the dfs function by passing arguments visited, graph and starting node.
7. Stop the program.
### Program:
```
graph={
    '2':['3','4'],
    '3':['5'],
    '4':['6','7'],
    '6':[ ],
    '5':['6'],
    '7':['8'],
    '8':[ ]
}
visited=[]
queue=[]
def bfs(visted,node,graph):
    visited.append(node)
    queue.append(node)
    while queue:
        m=queue.pop(0)
        print(m)
        for neighbour in graph[m]:
            if neighbour not in visited:
                visited.append(neighbour)
                queue.append(neighbour)
print("BFS order is")
bfs(visited,'2',graph)

```
### Output:



![image]<img width="2560" height="1600" alt="image" src="https://github.com/user-attachments/assets/a90c8dc8-6475-4df0-955c-3c3d25390f51" />



### Result:
Thus the breadth first search order was found sucessfully.
