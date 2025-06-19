# To do's

## UI
* Remove all references from the scene files to numpy, convert to np.array in the class files itself
* Ipv checkbox een radiobutton voor full raytrace / ordered elements
* Display support (centroid, image, ...) for multiple sources
* Laser shape visualiseren
* Polaire plot in display opties
* Lens from svg or dxf file
* UI tabs in aparte files
* if __main__ overal implementeren
* 4 Meer en betere properties van items plotten
* 5 str__ methods overal standaardiseren
* Docstrings & documentatie
* Beweegbaar display:
	* Makkelijk te verplaatsen langsheen zijn normaal bv.
	* Interseccties enkel met rays die nog geen eindpunt hebben
* Console output in 4th tab "Console"
* Fifth tab with "about" or so
	
* DONE:
	* Laten werken zonder UI
	* Splash screen (see: https://stackoverflow.com/questions/58661539/create-splash-screen-in-pyqt5)
    * 3 Automatisatie:
        * UI opstarten met een bepaalde scene, en runnen
        * Allow for changing element properties:
           * After loading the scene: mss wat te complex
           * In main_console.py een parameter file schrijven en die dan inlezen in de load_scene of zo
        * Inzoomen op een bepaald deel van de grafiek
        * Een screenshot nemen van een bepaalde grafiek (canvas of canvasDisplay)
        * Afsluiten
	
## Raytracing features
* 1 Scatteren op diffuse oppervlakken doen met importance sampling (cumsum etc) en equal intensities, ipv random en weighed intensities
* 2 Virtual rays enkel mogelijk wanneer de "full raytrace" aanstaat ipv de snelle met "ordered items"
* Imager response implementeren & plotten
* Andere definities van N toelaten voor dispersie
* pre-defined glass property list
* Reflecties aan glas elementen implementeren

* DONE:
	* Back-tracing van bv. centroid, m.b.v. virtual sources
	* Rays exporteren naar txt file, in een bepaald formaat
    * Bewaar in de ray zelf de relatieve display coordinaat, en pixel nummer
	* Imager resultaat exporteren (centroid, ...)
	* Full, slower, non-sorted-slements raytracing
	
## Elements
* Diffuse sphere			
* Filter
* 6 IdealThickLensClass
* Glass sphere
* Single ray source
* Aspherical lens
* Diffractive elements (aan de randen)
* Microlens
* Fresnell
* Biprism
* Powell lens

* DONE:
	* Ideal thin lens class
	* Spherical lens
	* Diffuse plate
	* Glass plate
	* Flat mirror
	* Parabolic mirror
	* Mirror only one side reflective
    * Semi-transparent mirror

## Varia
* Documentation
* Example files