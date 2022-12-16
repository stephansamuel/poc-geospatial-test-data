# Generate Sane Geospatial Test Data (Proof of Concept)

Outline:

- Open a geospatial data source and figure out what it contains and how to retreive data from it.
- Inspect the list of layers.
- Find the layer that contains the most data. Create an object for this as a reference because we will probably support multiple layers in the future.
- Also, allow the layer of choice to be configured.
- Determine the geometry of shapes within the layer to use.
- Figure out the average, "mass," of an object. This is trivial if the geometry is (single-)point.
- Figure out the extents of the layer.
- Extrapolate a subset extent. Use a base relative size of 10% but allow configuration of this and other parametric measures.
- Figure out the, "density," of objects.
- Figure out average span per object and average spacing. Use delta-x and delta-y to determine OA size and average distance to 3 closest neighbors for spacing.
- Use a parametric modeler to generate a new shape.
