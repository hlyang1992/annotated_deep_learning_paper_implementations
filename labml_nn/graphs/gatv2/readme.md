# [Graph Attention Networks v2 (GATv2)](https://nn.labml.ai/graph/gatv2/index.html)

This is a [PyTorch](https://pytorch.org) implementation of the GATv2 opeartor from the paper
[How Attentive are Graph Attention Networks?](https://arxiv.org/abs/2105.14491).

GATv2s work on graph data.
A graph consists of nodes and edges connecting nodes.
For example, in Cora dataset the nodes are research papers and the edges are citations that
connect the papers.

The GATv2 operator which fixes the static attention problem of the standard GAT: 
since the linear layers in the standard GAT are applied right after each other, the ranking 
of attended nodes is unconditioned on the query node. 
In contrast, in GATv2, every node can attend to any other node.

Here is [the training code](https://nn.labml.ai/graph/gatv2/experiment.html) for training
a two-layer GAT on Cora dataset.

[![View Run](https://img.shields.io/badge/labml-experiment-brightgreen)](https://app.labml.ai/run/8e27ad82ed2611ebabb691fb2028a868)