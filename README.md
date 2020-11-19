# new3
ex1 README
@auther Tehila Abadi

 File list
-----------------
node_info1			node_info implementation (private class)
WGraph_DS			weighted_graph implementation
WGraph_Algo			weighted_graph_algorithms implementation
WGraph_DSTestMine		unit test file for WGraph_DS and ndoe_info1
WGraph_AlgoTestMine		unit rest file for WGraph_Algo
README 				this file

_Introduction_
node_info1 class
Implements the interface of node_info.
represents the node (vertex) and all its properties in a weighted undirected graph.			

WGraph_DS
Implements the interface of weighted_graph.
Represents wighted undirected graph and all its properties.

WGraph_Algo
Implements the interface of weighted_graph_algorithms.
Represents the algorithems on a weighted undirected graph.

_Functions implemets_
node_info1 class:
This object contains a unique key, Int tag, and String info.
node_info1 is a private class of WGrpah_DS.

WGraph_DS class:
This class contains HashMap=graph- represents all the nodes in te graph.
HashMap of HashMaps contains each node in the graph as the key, and a HashMap of his neighbors as the object.
Another HashMap of HashMap for eacg edge in the graph and its weight.

public boolean hasEdge(int node1, int node2):
This method returns true iff (if and only if) there is an edge between node1 and node2

public double getEdge(int node1, int node2) :
This method returns the weight of the edge between these two nodes.

public void connect(int node1, int node2, double w):
This method connect between two given nodes with a given weight. If the nodes already connected the function updated the weight of the edge.

public Collection<node_info> getV():
returns a collection of all the nodes in the graph.

public Collection<node_info> getV(int node_id):
returns a collection of all the neighbors of the given node id.

public node_info removeNode(int key):
removes the node from the graph and delete all its edges.

public void removeEdge(int node1, int node2) :
removes the edge between the two given nodes.

WGraph_Algo:
 This class implements the interface of weighted_graph_algorithms represents an 
 Undirected (positive) Weighted Graph Theory algorithms including:
 deep copy
 init(graph);
 isConnected();
double shortestPathDist(int src, int dest);
List<node_data> shortestPath(int src, int dest);
Save(file);
Load(file);

public weighted_graph copy():
This method creats a new identical graph to the current graph.

 public boolean isConnected():
This mehod returns true if and only if this graph is connected.

public double shortestPathDist(int src, int dest) :
This method calculates the shortest path between two given nodes in a weighted graph

 public List<node_info> shortestPath(int src, int dest) :
this method returns a  list of all the nodes in the shortest path between the two given nodes.

public boolean save(String file):
This method saves this weighted graph to the given file name

public boolean load(String file):
This method load a graph to this graph algorithm from the given file name.
