# Potential flow visualizer

Takes in parameters of potential flow elements, calculates the flowfield around them, and returns a figure and axes containing the magnitude of velocity as a color contour and the plotted streamlines. Gives the option to specify the density of the streamlines and whether or not to automatically plot the visualization or not.

# Example usage
fig, ax, _, _, _ = potflow([["ufl", [0], 10], ['dbl', [0,0], 10],['vor', [0,1], 10]], levels = 50, visualize=False)
fig.canvas.draw()
plt.pause(0.1) 
input("Press Enter to close...")
plt.show()
