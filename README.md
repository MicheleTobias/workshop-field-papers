# Participatory Mapping with Field Papers
This workshop explores using [Field Papers](http://fieldpapers.org/) for participatory mapping.

## Learning Objectives

By the end of this workshop, participants should be able to

1. Understand the advantages and disadvantages of using the Field Papers tool
1. Be aware of some of the etiquette of participatory mapping and consider common concerns associated with participatory mapping
1. Set up a Field Papers Atlas
1. Collect data on a Field Papers Atlas
1. Georeference Atlas pages with the online uploader tool
1. Understand options for working with the georeferenced images

# What is Participatory Mapping?
Participatory mapping is a set of techniques that combines traditional cartographic methods with participatory methods to document the knowledge of a community.  The methods can take many forms but can include discussions, marking places on maps, or in-field data collection with GPS.  The end goal is to produce a physical map or digital dataset containing local geographic knowledge.

For example, a community might want to document places they feel are unsafe because of a lack of functioning street lights.  To solve the problem, they first need to understand the scale of the problem - how many sites are problematic and where are they?  They might get a map of their community and have people draw on the map where they think the problem areas are.

In this workshop, we'll be using a printed map workflow to collect our knowledge of some aspect of the UC Davis campus.

# What is Field Papers?
What is [Field Papers](http://fieldpapers.org/about)?  Field papers is an online tool built by [Stamen Design](http://www.stamen.com/) that manages the participatory workflow that uses printed maps to collect information from printing maps, to georeferencing, and finally data digitizing using [OpenStreetMap](https://www.openstreetmap.org/) editing tools or importing into your own GIS program.

![alt text](/images/atlas_pages.jpg "Printed Atlas Pages Arranged Together")

## Workflow Overview
A typical printed map participatory mapping workflow includes these steps:

1. **A Physical Map** - The map could be from any source - a travel map, a USGS Topographic Quadrangle, a print out from OpenStreetMap
1. **Write on the Map** - Community members draw and write on the map to indicate locations of the locations that are important to them.
1. **Scan or Photograph the Map** - You'll need to make your analog map into a digital image by scanning or taking a picture with a digital camera.
1. **Georeference** - Georeferencing is the process of adding geographic coordinates to a scanned map image so that it can work with other spatia data.  Field Papers does this for you when you upload your map images.
1. **Digitize Data** - Create vector data from your scanned, georeferenced map for use with other spatial data.  Depending on your goals, this step may not be necessary.


## Further Considerations

This workflow with Field Papers works well when:

* The community has map-reading skills already or you can train them
* The community feels comfortable collecting knowledge in this way
* The data generated is not sensitive or private
* The community wants to contribute their data to collaborative datasets like OpenStreetMap

Other things to consider: This kind of data collection can feel extractive to some communities.  Be sure you can explain how the data will be used and stored.  To be truly participatory, the community should have ownership of their data and it should help or be of value to them, not just the researcher.  Additionally, you'll want to be careful to protect the data you collect and consider how mapping a set of knowledge might impact the community.  For example, making the locations of important cultural sites public can expose the area to looting or damage.  

Like many universities and agencies that do research, UC Davis requires that research involving human subjects complete the research review process with the [UC Davis Institutional Review Board (IRB)](https://research.ucdavis.edu/policiescompliance/irb-admin/).  Participatory mapping methods require review.

**This workflow is not appropriate for personally indentifiable information (PII), HIPAA-restricted data, or data that should not be shared with a third party.**

# Hands On Lesson

## Making an Atlas

An atlas is a continuous map printed over several individual sheets of paper.

On the [Field Papers Compose page](http://fieldpapers.org/compose#15/38.5383/-121.7558), use the tools to set up your atlas.  Center your map in the location you would like to map, and use the tools in the upper left corner of the map to design the layout of the pages that will comprise your atlas.  You can change the scale (zoom level) and the number of columns and rows of pages.  The options of the left side of the screen let you change the paper size, orientation, and basemap. (A side note, the black and white background looks good on the screen, but the gray may not print well on some printers, so do a test before you print a bunch of pages.)

When you're happy with your Atlas specifications, click the 'make atlas' button.  It may take a few minutes to process.  When it is done, click the 'Download PDF' button to save the file with your atlas pages.  You'll need to print this file to work with it.  (A side note: make sure you turn off duplexing on your printer, especially if you want to tape the pages together into one big map.)

We've made an example atlas for you in the [Data folder](/data) of the UC Davis campus.


## Marking up the Atlas

Together, let's decide on what we want to mark on our map.  If you're doing this exercise to collect data about a specific question, your decision is made for you.  For the purposes of this workshop, we can map anything we like.

Some ideas include:
1. Nice walks on campus
1. Places to view campus wildlife
1. Pleasant places to eat lunch
1. Places to take your parents or friends when they visit

How will we map these things?  Let's decide on how we will indicate each of the things we are interested in.  Will we use one color for each topic?  Or a specific icon - a star, for example? Or do we want to place a sticker?  Deciding on cartographic rules before you start can save some confusion and trouble later on.

## Photographing or Scanning Atlas Pages

Once we have information written on our atlas pages, we need to make a digital copy of the pages.  We can do this by taking a photo (phones work!) or scanning the pages with a digital scanner.

|Format|Pro|Con|
|---|---|---|
|Photo|Phone cameras are readily available|Quality may be an issue|
|  |Cloud storage facilitates data transfer  |Stretch at photo edges distorts images|
|Scanner|Control image quality|An additional cost (solution: see GIS room on lower level of Shields)|
|  |Scanner lid flattens pages, less image distortion| |
|  |No shadows| |

Transfer the images to your computer. If you're using your phone, cloud photo services or online storage services can make this easy. (I'm letting my android phone upload the photos to Google Photos, then downloading them from my online account to my computer's hard drive.)

We have uploaded example photographs in the [a folder in the Data Folder](/data/Example_Data_Photos) along with cropped and rotated photos in [this folder](/data/Example_Data_Photos_Cropped).

![alt text](/data/Example_Data_Photos_Cropped/A2_cropped.jpg "One Page of the Atlas Scanned and Cropped")

## Georeferencing

The big advantage of using Field Papers is that the online tool can automatically georeference the atlas pages because of the marks embedded in the images (notice the plack circles and QR code along the edges of the map).

On the [Field Paper Upload page](http://fieldpapers.org/snapshots/new), upload one of your images.  When it finishes, the interface will offer you several options for working with the file.  We want to click 'Download GeoTIFF' to get a file we can use in a GIS.  The options below that (iD, Potlatch, JOSM) are ways to view the image in an OpenStreetMap (OSM) editor to digitize into the OSM dataset.  This is a nice way to contribute data to the shared OSM dataset, but if we're working on a research question, the data we generate might not be useful to the broader OSM community and might not be something we want to share publically. 

What if my image doesn't process?  Try these things:
1. Take a new image as close as you can, avoiding shadows
1. Make sure your image is in focus
1. Make sure your image is taken as perpendicular to the page as possible (nadir, not obique)
1. Crop the edges off of the image, making sure not to remove the reference points or QR code.

We have uploaded example geocoded photographs in the [Data Folder](/data/Example_Data_Photos_Georeferenced).

## GIS Work

Now we can open our favorite GIS, import our georeferenced atlas pages, and trace the places we mapped.

In the workshop, we'll be working in [QGIS](https://qgis.org/) to create vector data from our scanned and georeferenced maps.  The QGIS Training Manual's [Creating Vector Data](https://docs.qgis.org/3.4/en/docs/training_manual/create_vector_data/index.html) module is an excellent intoduction to this workflow.

![alt text](/images/QGIS_atlas_pages.png "Georeferenced Atlas Pages in QGIS")

Generally, we'll use this workflow:

1. Open QGIS
1. Load the georeference map data
1. Create a new, empty vector dataset to hold our edits - being sure to pick the correct geometry type (points, lines, or polygons). Note that we may need multiple files - one for each geometry type we need to work with.  Add the attribute columns we want to describe the marks - we might want a Name column or a column to contain counts at the site... it depends on what we decide to map.
1. Use the digitzing tools to trace our marks
1. Import other background data to help us interpret our spatial distribution
1. Style the data we created
