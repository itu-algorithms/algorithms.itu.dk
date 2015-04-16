---
category: events
title: Ilya Razenshteyn - Optimal Data-Dependent Hashing for Approximate Near Neighbors
time: April 21, 10.30-11.30
place: Room 3A08, ITU.
---
The classic Approximate Near Neighbor problem (ANN) can be formulated as follows. Given a dataset of points the goal is to preprocess it so that, given a query point close to some data point, return a data point that is not too far from the query. If one insists on the space being subquadratic in the number of points (the most important regime in practice), the only known technique for tackling ANN until recently was Locality-Sensitive Hashing (LSH) introduced by Indyk and Motwani in 1998. Since then, LSH has been proved very influential both in theory and in practice.

During the talk, I will introduce LSH and state certain fundamental limitations of it. Then, I will talk about a recent line of work that overcomes them. That is, I will show first data structures for ANN that are provably better than the best possible LSH-based ones. In particular, for the first time, we are able to improve upon [Indyk-Motwani 1998] for the Hamming distance, and [Andoni-Indyk 2006] for the Euclidean distance.

The key technique is *data-dependent hashing*: we tailor the hash family to a given set of data points; this approach has strong parallels with the practice of ANN. Our hashing schemes are *optimal* in the class of data-dependent hashing. The key technical tool is a regularity-type decomposition: we show how to partition a *worst-case* dataset into several parts that look *random*.

The talk is based on a joint work with Alex Andoni (Simons Institute) that can be found at http://arxiv.org/abs/1501.01062​.