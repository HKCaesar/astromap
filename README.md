# astromap

geocoded location, altitude, IAU code, principal instruments, 
organization, targets/science, website, and photo of selected 
astronomical observatories. "optical.kml" and "radio.kml" are
merged into "astromap.kml".

 *  astromap is not a map. it's a description of places in KML
    which can be loaded into many mapping applications, e.g.
    Google Maps or Bing Maps.
 *  it does not contain all known telescopes, nor even all 
    known observatories. it's a selection of major observatories
    often hosting many telescopes.
 *  it is intended to complement [more complete][1] observatory 
    maps and lists with more or less information in a short 
    summary and a photo.
 *  it is a subset (but hopefully representative) of:
    *  List of Observatories, Wikipedia
    *  List of largest optical reflecting telescopes, Wikipedia
    *  List of largest optical refracting telescopes, Wikipedia
    *  List of Radio Telescopes, Wikipedia
    *  Large Telescopes, Nine Planets
    *  Historic Astronomical Sites, NOAO

[1]: http://www.eso.org/~ndelmott/obs_sites.html


# format

observatory names have the form:

    name | elevation in meters | [IAU code]

observatory descriptions have the form:

    location | instruments | organization | mission | website


# you can help

if you would like to point out an error, ommission, improvement, 
or can contribute a translation, please let me know.

if you are a programmer, you can make contributions by forking 
this code and submitting a patch via Github.


# F.A.Q.

## where can I download the astromap KML directly?

<https://raw.github.com/siznax/astromap/master/astromap.kml>

## how can i view the map in Google Maps?

there are at least three ways, you can

1. Specify the KML file as a query parameter.
   eg. <http://maps.google.com/maps?q=https://raw.github.com/siznax/astromap/master/astromap.kml>, or 
2. create a map in "My Places" and import the _astromap_ KML file, or 
3. create an HTML page with <code>google.maps.KmlLayer(kml)</code>
   see eg/layer-google.html

## how can i view the map in Bing Maps?

there are at least three ways. you can

1. Specify the KML file as a query parameter.
   eg. <http://www.bing.com/maps/?mapurl=https://raw.github.com/siznax/astromap/master/astromap.kml>, or 
2. specify a Google map URL as a query parameter
   <code>http://www.bing.com/maps/?mapurl={gmap_url}</code>, or
3. create an HTML page with <code>VEShapeSourceSpecification</code>
   see eg/layer-bing.html

## where is the KMZ file?

1. You can create one on GPS Visualizer from the KML file.
