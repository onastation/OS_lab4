# OS_lab4
Analysis of the properties of an unweighted bipartite graph in solving the problem of finding the maximum pair connection allows us to formulate the following theorem.

**Theorem 1:**

If in the matrix RJ [i, j], i = 1..N, j = 1..N of the graph G = (VR, VJ, E), where VR = {1,2 ... N}, VJ = { 1,2 ... N} there is a solution. A power n = N and there are such vertices (p, q) that:

RJ [p, q] = 1,

RJ [p, j] = 0 j {1 .., N} \ q and / or

RJ [i, q] = 0 i {1 .., N} \ p.

Then this pair (p, q) always participates in the solution A (p, q) A.

(In other words, if for an unweighted bipartite graph there is a perfect pair and the graph has a vertex with degree one, then the edge incident to this vertex and the vertices incident to this edge must be included in the perfect pair)

**Conclusion 1.**

If there is a solution A \*, then the assignment task can be divided into two parts: in the first part only mandatory assignments (p, q) are involved, in the second part - the remaining assignments from the new connectivity matrix MC \*, which can be obtained after deleting the rows and columns corresponding to the mandatory purpose defined by Theorem 1.

**Theorem 1 \***

Any of the vertices of an unweighted bipartite graph, having a degree equal to one, always participates in one of the variants of the maximum pairing.

**Theorem 2.**

If in the matrix RJ [i, j], i = 1..N, j = 1..N, FA (fan) and:

FA = {(R1, q), (R2, q), ..., (Rf, q)}, Rk {1, .., N}, 2 f N, where RJ [Rk, q] = 1 for k = 1..f and RJ [Rk, Jk] = 0, Jk {1, .., N} \ q (2.7) or

FA = {(p, J1), (p, J2), ..., (p, Jf)}, Jk {1, .., N}, 2 f N, where RJ [p, Jk] = 1 for k = 1..f and RJ [Rk, Jk] = 0, Rk {1, .., N} \ p (2.8),

then any of the vertices FA is included in one of the variants of the maximum pairing, the assignment task does not have a complete solution and the power of the maximum pairing M \&lt;N-f + 1.

**Conclusion 2**

The dimension of the solution of the problem of finding the maximum pairing can be reduced by the number of pairs of vertices defined by Theorems 1 and 1 \* and the search for the pairing must be conducted from a new graph

**Conclusion 2 \***

The dimension of the solution of the problem of finding the maximum pairing should be reduced by the number of vertices included in the fan, and the search for the pairing should be conducted from a new graph.

**Conclusion 3**

Adjacent edges incident to the vertices defined by Theorems 1,2 should be removed from further consideration, and the initial graph is reduced and transformed into a new graph.

 Theoretical prerequisites for the allocation of conflicting appointments

Analysis of the properties of the bipartite graph shows that together with the mandatory assignments in it we can identify &quot;conflicting&quot;, which fall into the solution (basic or initial version of the solution is random) inevitably leads to the appearance of free vertices (not included in solution), and hence to additional steps in the formation of the final solution.

The localization of conflicting assignments is realized on the basis of the equivalent transformation of the initial graph, which is an isomorphic transformation, which consists in the target permutation of rows and columns of the connectivity matrix. In developing the algorithm, the following obvious statements were taken into account, which do not require proof.

**Proposition 1**

Since each line of the CU is a reflection of the possible distribution of resource requests, the change of places of the two lines of the CU with memorization of the new location of the requests does not affect the qualitative characteristics of the CU and the initial graph.

**Proposition 2**

Since each column of the CU is a reflection of the claim for applications to capture this resource, the change of places of the two columns of the CU with memorization of the new location of resources does not affect the qualitative characteristics of the CU and the initial graph.

**Theorem 3**

If after the equivalent transformation of the CU it is possible to obtain the term rank of the CU equal to the rank of the CU, then all applications have destinations corresponding to &quot;1&quot; of the main diagonal and: found a complete combination, obtained one of the

**Theorem 4.**

If in the matrix MS [i, j], i = 1..N, j = 1..N we can select the submatrix MM [k, l], k = 1..T, l = (N-S + 1). .N, where S + T\&gt; N and MM = (- zero matrix), then the assignment problem does not have a complete solution.

**Theorem 5.**

If in the matrix RJ [i, j], i = 1..N, j = 1..N, we can select the submatrix MN [k, l], k = 1..T, l = (N-S + 1) ..N, where S + T = N and MN =, then for Ri {1, .., (NS)}, Jj {(T + 1), .., N}: (Ri, Jj) A. All (Ri, Jj) A

**Theorem 6**

If in the matrix MT [i, j], i = 1..N, j = 1..N, several submatrices satisfying Theorem 5 can be distinguished, then all corresponding submatrices symmetric with respect to the main diagonal are &quot;conflicting&quot; and must be reset.

**Results:**

![](https://user-images.githubusercontent.com/43548404/103959712-1b7c4400-5159-11eb-8781-f2169ebf14b4.png)
