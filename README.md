Readme

This is a Python-based project that utilizes the PyTorch Geometric, NetworkX, matplotlib, and PyVis libraries to create and visualize graphs. The data used to generate these graphs comes from surgical video frames, and the graphs represent relationships between instruments and anatomical structures within these frames.
Dependencies

    Python 3.7+
    PyTorch 1.6.0+
    PyTorch Geometric 1.6.1+
    NetworkX 2.5+
    matplotlib 3.3.2+
    numpy 1.19.2+
    glob2 0.7+
    plotly 4.12.0+
    PyVis 0.1.9+

Data Preprocessing

The load_data function is used to load the data from .txt files. These files contain information about surgical instruments and anatomical structures identified in each frame of the surgical video.
Graph Creation

The build_pyg_graph function takes the loaded data and constructs a graph using PyTorch Geometric. Each node in the graph represents a frame, an instrument, or an anatomical structure, and the edges represent the relationships between these entities.
Visualization

Several functions are provided for visualizing the graph:

    visualize_networkx_graph: This function uses NetworkX and matplotlib to create a static 2D graph visualization.
    visualize_networkx_graph_interactive: This function uses NetworkX and plotly to create an interactive 2D graph visualization.
    visualize_pyvis_graph_interactive: This function uses PyVis to create an interactive 2D graph visualization with custom node positions. The layout_func parameter can be used to specify a custom layout function for the nodes.

Running the Code

The main section of the code demonstrates how to use these functions with a specific example data set. You will need to modify the file paths for your specific data.
Note

The data used in this project is expected to be in a specific format. Please ensure that your data matches this format for the code to run correctly. You can refer to the load_data and build_pyg_graph functions for more information about the data format.

Created using GPT4
