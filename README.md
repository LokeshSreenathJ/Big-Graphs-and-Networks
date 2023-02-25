# Big-Graphs-and-Networks
1)Minimium Spanning Trees:
  Used Dataset : http://konect.cc/networks/adjnoun_adjacency/
  Built Minimum Spanning Tree  model using Prim's and Kruskal's algorithm from scatch using numpy library in Python.
  
2)is_dag():
  Built a model that tells us whether a given graph is Directed Acyclic or not a DAG. Being a DAG for any graph has a wide applications one prominent that I have witnessed is in Scheduling and Order Processing from warehouse to customers.
  
3)make_dag():
  We wish we have a DAG graph but it isn't the case always. To make a Cyclic graph to acylic 1) Identify the disjoint components of graphs  2) Examine each component if it has a cyclic then it remove the edges till you reach number of edges as N-1 , where N represents the number of nodes in that paticular component of graph.
  
4)sort_dag():
  Having the node ordered in topologically have many utilities. In order to get the nodes that have a uni direction of edges terminating from it from left towards the right side or vice-versa, 1) Try identifying the node that has no incoming edges. If you find one, append it to the node_order list, then remove the  nodes associated with that paticular node. 2) Repeat this for all the nodes. 
  
5)Finding the Shortest Path Problem:
  Used Dataset :https://people.sc.fsu.edu/~jburkardt/datasets/cities/cities.html. 
  Graph construction: Constructed weighted undirected network (edges weighted by distances) with each city forming a node, and an edge (i,j) exists between two cities if i) the distance between i and j is not greater than 100 miles, or if ii) there are no cities within 100 miles from a city i, add an edge from i to its nearest city.
  This dataset contains the distances between the cities of USA (The distance values used are not accurate though). Built dijkstra's algorithm from scatch using numpy library in python. The graph obtained from above constaints results in dis-connected graph. I have considered the case of dis-connectednesss of graph and developed the algorithm.
  Also using Floyd-Warshall Algorithm developed a model that gives us the distance matrix which contains the all-pairs shortest possible distances between all cities.

6) Maximum Flow between source and destination:
  Input dataset : http://snap.stanford.edu/data/soc-sign-bitcoin-otc.html
  Graph Construction: Considered nodes from 1 to 2000 and non-negative edges. Built the Maximum flow algorithm that can find the maximum amount of flow between source and destination.
