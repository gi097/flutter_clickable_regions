# Flutter clickable SVG regions (Interactive Map)
[![Build Status](https://travis-ci.com/gi097/flutter_clickable_regions.svg?branch=develop)](https://travis-ci.com/gi097/flutter_clickable_regions)
This is a simple application which displays an SVG image with clickable regions.
It displays all the provinces from The Netherlands. When you click on it, 
it will display the name of the clicked province.

## Getting Started
Get a SVG and open it in a text editor. In this example, we are using the SVG image
from https://mapsvg.com/maps/netherlands/.

The file will show several ```<path></path>``` entries. You need to add these manually
in all the `@SvgPath` annotations.

After adding the annotations, you can run the below command to generate the needed
`Path` objects.

```bash
flutter packages pub run build_runner build
```

## Known issues
Some provinces are not clickable. This is an issue of the SVG being used.

## Screenshot
![Screenshot](images/map.gif?raw=true)

## Author
Giovanni Terlingen <me@giovanniterlingen.com>
