PngThumbnail
============

Squish images using pngquant, then pngout, with a perceptual difference check at the end.  All wrapped up in a Platypus droppable mac app, but the basic script is just a shell script.

Passes dropped image files through pngquant at thumbnail quality, then through pngout.  Finally compares the files using perceptualdiff with a FOV appropriate for handheld phone distance.  All modified files go in a out/ subdir of the input file. If the diff fails, the perceptual diff output is included (converted to a png using gm (graphicsMagick, which must be installed separately), along with a copy of the original image.

The app bundle itself contains pre-built binaries for everything needed EXCEPT for graphicsMagick, which you can install using your favorite method.
