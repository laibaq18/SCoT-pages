# Cluster-Analysis-Menu

[Back to user guide contents list](userGuide.md)

After clicking the Analyse Clusters button in the navigation bar, SCoT opens the Cluster Analysis Menu on the right-hand side of the screen. This panel allows users to inspect, compare, edit, and analyze the clusters generated from the graph.

![Analysis Menu](./images/main-right-bar.png)


## Contents
* [Editing the Clusters](#editing-the-clusters)
* [Edit Cluster Name](#edit-cluster-name-&-colour)
* [Edit Cluster Colour](#edit-cluster-name-&-colour)
* [Nodes Plot](#view-nodes-plot)
* [Cluster Context Analysis](#cluster-context-analysis)
* [Add Cluster Node](#add-cluster-node)
* [Delete Cluster Node](#delete-cluster-node)
* [Delete Complete Cluster](#delete-complete-cluster)


[To the top](#editing-the-graph-via-the-functions-of-the-editing-sidebar)

## Editing the Clusters

Each cluster is displayed as an expandable panel in the analysis menu.
For every cluster, SCoT provides:
* the number of nodes in the cluster,
* a nodes plot,
* option to change cluster name/color,
* option to show the context-words that are shared by all nodes of the cluster,
* and cluster deletion functionality.

Clusters are colour-coded and correspond directly to the colours used in the graph visualization.


![Cluster List](./images/nodes-detail.png)

When hovering over the cluster and context buttons, all the nodes and edges in the graph belonging to the cluster are faded in in the graph.

![Fade In Cluster](./images/hover-over-a-cluster.png)


In some cases, nodes are not connected to any other in the graph. They are only neighbours of the target word. Then, the nodes are not rendered in the graph, but they are listed under "Singletons" in the edit column.

![Singletons](./images/singleton.png)


## Edit Cluster Name & Colour

The program only numbers the clusters and it is up to the user to name the cluster. Users can rename clusters and also assign custom colours through the Name section.

The user can:
* change the cluster name,
* display the cluster label inside the graph,
* and select a custom cluster colour using the colour picker.

![Edit Cluster Name & Colour](./images/cluster-name-color.png){:height="40%" width="40%"}

The user can enter the new name in the text input field "Change cluster name". The name of the cluster is automatically updated while typing. The user can also select a different cluster colour by clicking on the colour field with the label "Select cluster colour" when editing a cluster. Then a colour picker opens and the user can select the new colour. Your colour picker may look different to the one in the image, since the appearance of the colour picker depends on your browser. The colour of the circle next to the cluster name is directly updated. 

However, the graph updates with the new name and color after clicking "Update Clusters" at the bottom of the analysis panel. The user can edit multiple clusters before clicking the "Update Clusters" button to make the updated visible in the graph.

[To the top](#editing-the-graph-via-the-functions-of-the-editing-sidebar)

## View Nodes Plot

The Nodes Plot shows the aggregated average frequency and similarity of cluster nodes across different time intervals. It helps users observe how strongly connected and how frequently used the cluster terms are over time.

Users can also compare multiple clusters in the same plot by selecting "Add other clusters" from the list below the graph. This makes it easier to identify semantic trends, changes in importance, and similarities or differences between clusters over time.

<p align="center">
  <table>
    <tr>
      <td align="center">
        <img src="./images/nodes-plot-1.png" alt="Single cluster nodes plot" width="100%">
        <br>
        <em>Single cluster nodes plot</em>
      </td>
      <td align="center">
        <img src="./images/nodes-plot-all.png" alt="Multiple cluster comparison plot" width="100%">
        <br>
        <em>Multiple cluster comparison plot</em>
      </td>
    </tr>
  </table>
</p>

Users can interact with the graph by "zooming-in or zooming-out" and can also download the generated plot via the "camera icon" at the top. 

## Cluster Context Analysis

The context section shows the most significant syntagmatic contexts of the nodes of a cluster.

![Cluster Context](./images/cluster-context.png)


By clicking the "Context" button, a table opens to the left which contains context-words, normalized significance score, and filtering options. By selecting context-words and clicking “Context-Frequency Plot”, users can generate a temporal visualization of context frequency over time. This plot helps users analyze when a context emerged, how important a context became, and whether a context increased or declined historically.

The selected context words are listed below for reference.

![Cluster context table](./images/cluster-context-bar.png)
![Cluster context frequency plot](./images/cluster-context-plot.png)


Users can filter the context-words using the search field to focus on specific semantic patterns of a target word. Calculations can take long. It is recommended to query only clusters with 20 or less nodes.

![Filtered context words](./images/context-filtered.png)


## Delete Complete Cluster

Complete cluster can be deleted via the button with the trash icon. The user then has to confirm the deletion in a confirmation message. When the user confirms all the nodes and links of the cluster are deleted.

![Confirm Cluster Deletion](./images/delete-cluster.png){:height="75%" width="75%"}


## Add Cluster Node [currently under revision - not enabled]

The user can also add a special node with the cluster name to the graph for each cluster - sort of like a label for a cluster. This node has edges to all the other nodes in the cluster.

![LABELED GRAPH](./images/graph_with_labels.png)

To add a new cluster label, the user ticks the box "Show cluster label in graph" when editing a cluster and clicks the "Apply" button at the bottom of the edit column.

![TICKED LABEL BOX](./images/ticked_box_label.png)

For each cluster only one cluster node can be added.

When reclustering the graph, the old labels are kept in the graph. Since the reclustering produces new clusters on the graph, the user can add new cluster labels. The old labels are kept, so that the clusters can be more easily compared. When hovering over a cluster node, all the nodes connected to it (i.e. all the nodes in the cluster) are faded in.

The same behaviour is displayed when updating the graph.

[To the top](#editing-the-graph-via-the-functions-of-the-editing-sidebar)


## Delete Cluster Node

In case the user wants to get rid of the cluster node of a cluster, they have two possibilities. Both are explained in [the section on interacting with the graph](interacting.md).

[To the top](#editing-the-graph-via-the-functions-of-the-editing-sidebar)

[To the top](#editing-the-graph-via-the-functions-of-the-editing-sidebar)
