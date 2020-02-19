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


# What is Field Papers?

## Workflow Overview

## Pros & Cons


# Hands On Lesson

## Making an Atlas

An atlas is a continuous map printed over several individual sheets of paper.

On the [Field Papers Compose page](http://fieldpapers.org/compose#15/38.5383/-121.7558), use the tools to set up your atlas.  Center your map in the location you would like to map, and use the tools in the upper left corner of the map to design the layout of the pages that will comprise your atlas.  You can change the scale (zoom level) and the number of columns and rows of pages.  The options of the left side of the screen let you change the paper size, orientation, and basemap. (A side note, the black and white background looks good on the screen, but the gray may not print well on some printers, so do a test before you print a bunch of pages.)

When you're happy with your Atlas specifications, click the 'make atlas' button.  It may take a few minutes to process.  When it is done, click the 'Download PDF' button to save the file with your atlas pages.  You'll need to print this file to work with it.  (A side note: make sure you turn off duplexing on your printer, especially if you want to tape the pages together into one big map.)

We've made an [example atlas](data\atlas-3hasivcl.pdf) for you in the Data folder of the UC Davis campus.

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
|Scanner|Control image quality|harder to come by (solution: see GIS room on lower level of Shields)|
|  |Scanner lid flattens pages, less image distortion| |
|  |No shadows| |

Transfer the images to your computer. If you're using your phone, cloud photo services or online storage services can make this easy. (I'm letting my android phone upload the photos to Google Photos, then downloading them from my online account to my computer's hard drive.)

## Georeferencing

The big advantage of using Field Papers is that the online tool can automatically georeference the atlas pages because of the marks embedded in the images (notice the plack circles and QR code along the edges of the map).

On the [Field Paper Upload page](http://fieldpapers.org/snapshots/new), upload one of your images.  When it finishes, the interface will offer you several options for working with the file.  We want to clikc 'Download GeoTIFF' to get a file we can use in a GIS.  The options below that (iD, Potlatch, JOSM) are ways to view the image in an OpenStreetMap (OSM) editor to digitize into the OSM dataset.  This is a nice way to contribute data to the shared OSM dataset, but if we're working on a research question, the data we generate might not be useful to the broader OSM community and might not be something we want to share publically. 

What if my image doesn't process?  Try these things:
1. Take a new image as close as you can, avoiding shadows
1. Make sure your image is in focus
1. Make sure your image is taken as perpendicular to the page as possible (nadir, not obique)
1. Crop the edges off of the image, making sure not to remove the reference points of QR code.

## GIS Work

Now we can open our favorite GIS and import our georeferenced atlas pages.
