
Julia is a high-level, high-performance dynamic programming language for technical computing, with syntax that is familiar to users of other technical computing environments.

###Image packages in Julia 
Julia has a few packages aimed at image processing. We’ll start by looking at the **TestImages package**, which hosts a selection of sample images, then briefly visit the **ImageView** package before moving onto the Images package, which implements a range of functions for image manipulation.

###Testimages package
The TestImages package currently provides 25 sample images, which form a convenient basis for experimentation.
**Step 1**
We’ll load the archetypal test image.
**Step 2**
Of course, now that we’ve loaded that image, we’ll want to take a look at it. To do that we’ll need the **ImageView package**.
**Step 3**
You can optionally specify the pixel spacing as a parameter to *view()*, which then ensures that the aspect ratio of the image is conserved on resizing. There are various other bobs and whistles associated with view(): you can click-and-drag within the image to zoom in on a particular region;various simple transformations (flipping and rotation) are possible; images can be annotated and multiple images can be arranged on a canvas for simultaneous viewing.
###Image representation
Outside of the test images, an arbitrary image file can be loaded using **imread()** from the Images package. Naturally, there are also functions for writing images,** imwrite()** and **writemime()**.

###Imread command
imread() allows us to read the image. float32sc() changes the image into real values. The result could be a single matrix if the image is black/white, or a triple array that contains three matrices representing each color **(Red, Green, Blue)**. 