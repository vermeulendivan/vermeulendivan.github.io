---
layout: page
title: Features
permalink: /features/
---

There are 11 types of features which can be extracted from a stream network:

- Crossing or Intersection: If two lines cross each other (without a node)

![crossing](/images/features/crossing.png)

- Pseudo node: A node that has one upstream and one downstream node. The node is superfluous as it can be represented by one line instead of two.

![pseudo_node](/images/features/pseudo_node.png)

- Well or Source: A node that has one downstream node and zero upstream nodes.

![well](/images/features/well.png)

- Sink: A node that has no downstream node and one or more upstream nodes.

![sink](/images/features/sink.png)

- Watershed: A node that has more than one downstream node and zero upstream nodes.

![watershed](/images/features/watershed.png)

- Separated: Only one upstream node or only one downstream node and intersects with one or more other lines. Note that in the lines below, there is only one node under the star, the other line has no node at the position of the star.

![unseparated](/images/features/unseparated.png)

- Unclear bifurcation: It has more than one upstream and more than one downstream node, but the number of upstream and downstream nodes are same.

![unclear_bifurcation](/images/features/unclear_bifurcation.png)

- Distributary or Branch: It has more downstream nodes than upstream nodes. The minimum number of upstream nodes is one.

![branch](/images/features/branch.png)

- Tributary or Confluence: It has more upstream nodes than downstream nodes. The minimum number of downstream nodes is one.

![confluence](/images/features/confluence.png)

- Segment centre: Segment centre is the linear centre of a line. The tool finds the point in the line that is half way along the line.

![segment_center](/images/features/segment_center.png)

- Self Intersection: Same as intersection (crossing), but this time the line intersects with itself.

![self_intersection](/images/features/self_intersection.png)
