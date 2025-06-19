# Feature list

## Raytracing features
* Accurate raytracing for certain elements
* Approximate raytracing for segments-based descripted elements
* Fast raytrace mode for ordered elements or slow mode for full raytracing
* Dispersion of different wavelengths
* Tracking of ray phase information
* Simulation with UI or purely via console

## UI features
* Visual representation of simulated scene
* Color schemes: Wavelength dependent, rainbow, fixed
* Glass color depends on refractive index
* Scene creation via a Python script
* Loading/reloading of scene files
* Export of ray data and imager data to file
* Number of simulated rays configurable up to 10M rays
* Number of plotted rays configurable
* Auto-redraw ON/OFF after simulation
* Dark background mode
* Showing element properties ON/OFF
* Intensity-coded or equal-intensity-coded ray colors
* Axis ON/OFF
* Showing non-colliding rays ON/OFF
* Various display representation modes: scatterplot 1D/2D, image 2D, centroid, phase plot
* Zoom, pan and take screenshots of all graphs
* Line width of rays depends on number of plotted rays, for better visualisation

## Supported objects

### Light sources
* `Plane source` - Equidistant or random distribution
* `Point source` - Equiangular, Gaussian or random distribution
* `Laser beam` - Simplified, but correct beam width & intensity at point of impact

### Lenses
* `Spherical lenses` - Defined by radii R0 and R1 or by focal distance f
* `Ideal thin lens` - 
* `Ideal thick lens` - With principal planes
* `Aspherical lens` - 
* `Custom shape` - Generated from svg/dxf

### Glass elements
* `Slab` - 
* `Prism` - 
* `Fresnell prism` - 
* `Single microlens array` - 
* `Double microlens array` - 
* `Biprism` - 
* `Sphere` - 

### Diffuse objects
* `Diffuse plate` - Described with BSDF (diffuse & specular parameters)
* `Diffuse sphere` - 

### Mirrors
* `Mirror` - 
* `Half-transparent mirror` - 
* `Parabolic mirror` - 

### Displays
* `Passive display` - 
* `Imager` - With angular response

### Varia
* `Black surface` - 
* `Bandpass filter` - With angular response (blueshift)
* `Diffractive element` - 


