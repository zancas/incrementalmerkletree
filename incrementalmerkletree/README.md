incrementalmerkletree
=====================

This crate contains common utility types and testing infrastructure used in the implementation
of the `bridgetree` and `shardtree` crates.

Terminology
===========

Leaf:  An element of the ordered set that the tree is constructed "across".
Path:  An ordered set of connected nodes.
Connection:  The relation between the 2 inputs (parents) and 1 output (child) of the Merkle-hash used to construct the tree.
ancestral Leaves:  The set of leaves necessary to compute a node (via the Merkle Hash).
Ascending:  Towards the leaves.
Descending:  Towards the root.
Ancestor:  Any node on an ascending path from a non-leaf node "A" its Ancestral Leaves.
