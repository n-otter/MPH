# Stratifying multiparameter persistent homology

Here you can find code for computation of invariants for multiparameter persistence modules, as introduced in the paper Stratifying multiparameter persistent homology, by H. Harrington, N. Otter, H. Schenck and U. Tillmann, preprint available at https://arxiv.org/abs/1708.07390, henceforth referred to as HOST.

We have written code which takes as input a simplicial complex and
one-critical bi-filtration, and builds the associated chain complex in
the Macaulay2 package of Grayson and Stillman, available at:
http://www.math.uiuc.edu/Macaulay2/. Note that this
code can  easily be adapted to the case r>2 (so not necessarily a
bifiltration). One important note: in Macaulay2, the degrees for
a multigraded ring start, by default, with index zero, so output for
multigraded Hilbert series always appears with variables T_0,T_1. In
particular, when reading Hilbert series computations below and
comparing to the computations in HOST, T_i \mapsto t_{i+1}.



## Computation of homology of chain complex.

In the file <a href="https://github.com/n-otter/MPH/blob/master/homology
">homology</a> we provide code that takes as input a  simplicial complex together with a one-critical bifiltration and builds the  associated chain complex.



<a href="https://github.com/n-otter/MPH/blob/master/first_example">Here</a> we illustrate how to build a chain complex, and then how to compute a minimal presentation of the first homology for the bifiltration in Example  3.24 in HOST.




## Hilbert function and series, local cohomology.

<a href="https://github.com/n-otter/MPH/blob/master/hilbert">Here</a> we show how one can compute the Hilbert function and series, and display the Hilbert function as a table.


## Rank.

Here we provide a code to compute the rank of the module, using the reduction to a line of Section \ref{S:restriction to line}.
