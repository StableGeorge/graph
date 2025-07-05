# What is it?

Graph allows you to graph any mathematical function. It uses the Qt Framework so you'll need that installed too.
You can graph functions and points with a lot of customizability

# How to use the graph library

Below is an example graph file:

'''
from PyQt5.QtWidgets import QApplication
from PyQt5.QtCore import *                                  # Only neccessary for "addGraph(..., style=Qt.SolidLine)"
import graph                                                # The Library itself
import math                                                 # Many functions to play with

app = QApplication([])
plane = graph.XY_Plane(900, 800)                            # Set the plane and the window dimensions
plane.setMinMax(0,10,0    ,10)                              # Set the minimum-maximum values for x/y-axis
plane.addGraph(function=lambda x:x, color=(255, 0, 0))      # Set the function "y=x" with red color
plane.show()
app.exec_()
'''