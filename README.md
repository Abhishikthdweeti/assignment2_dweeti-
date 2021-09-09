# assignment2_dweeti-
# Abhishikth Dweeti
###### los vegas
Las Vegas is an internationally renowned major **resort city**, known primarily for its **gambling**, **shopping**, fine dining, entertainment, and nightlife. ... The city bills itself as The Entertainment Capital of the World, and is famous for its **mega casino-hotels** and associated activities.
<h3> Directions to my favourite place
<hr>
<ol> <li> Start from Maryville to Irving</li>
     <li>Then Irving to Denver</li></ol>
<ul> <li>Drinks </li>
     <li>Snacks</li>
</ul>       </h3>  </hr>

<a href=https://github.com/Abhishikthdweeti/assignment2_dweeti-/blob/main/AboutMe.md >AboutMe</a>
<hr><h4>Food and Beverages </h4>
<p>Food and Beverages, places where they are available and their cost.</p>
<table>
<tr>
<th> Food/Drink </th>
<th> Location </th>
<th>Cost</th>
</tr>
<tr>
<td> Milk </td>
<td> Hy-vee </td>
 <td>$1.96  </td>
</tr>
  <tr>
  <td>Pepsi</td>
  <td>Walmart</td>
  <td>$0.96</td></tr>
</table>
</hr>
<hr><h5>Quotes</h5>
<blockquote><q>If life were predictable it would cease to be life, and be without flavor -<i>Eleanor Roosevelt </i></q><br>
<q>The greatest glory in living lies not in never falling, but in rising every time we fall -<i> Nelson Mandela</i></q>
</blockquote >
</hr>
<hr><h5>Breadth-first search</h5>
<blockquote><q>Breadth First Traversal (or Search) for a graph is similar to Breadth First Traversal of a tree (See method 2 of this post). The only catch here is, unlike trees, graphs may contain cycles, so we may come to the same node again. To avoid processing a node more than once, we use a boolean visited array. For simplicity, it is assumed that all vertices are reachable from the starting vertex. 
</q></blockquote>
<a href=https://www.geeksforgeeks.org/breadth-first-search-or-bfs-for-a-graph>Source link for definition </a><br>

```
vector<vector<int>> adj;  // adjacency list representation
int n; // number of nodes
int s; // source vertex

queue<int> q;
vector<bool> used(n);
vector<int> d(n), p(n);

q.push(s);
used[s] = true;
p[s] = -1;
while (!q.empty()) {
    int v = q.front();
    q.pop();
    for (int u : adj[v]) {
        if (!used[u]) {
            used[u] = true;
            q.push(u);
            d[u] = d[v] + 1;
            p[u] = v;
        }
    }
}
```

<br>
<a href=https://cp-algorithms.com/graph/breadth-first-search.html >Source link for code </a>



</hr>