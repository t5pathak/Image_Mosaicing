# Image Mosaicing - Stitching multiple images toghther!

Mosaicing is one of the techniques of image processing which is useful for tiling digital images. Mosaicing is blending together of several arbitrarily shaped images to form one large radiometrically balanced image so that the boundaries between the original images are not seen. Any number of geocoded images can be blended together along user-specified cut lines (polygons). [Image mosaicing](https://ieeexplore.ieee.org/document/702214)

# Steps to be Performed
1. Use any feature detector and descriptor (e.g. SIFT) to find matches between two partially overlapping images. You can use inbuilt functions for this.
2. Estimate the homography matrix between the two images robustly.
3. Transform one of the images to the other’s reference frame using the homography matrix.
4. Stitch the two images together.
5. Repeat this for multiple images to produce a singly mosaic/panorama.
6. Demonstrate the results on different scenes from the given data.
7. Additionally, capture a set of overlapping images of a scene with your camera and report the results on the same.

# Functions Used
1. Stitch - used to stitch any two images
2. Ft_matches - feature matching
3. RandCons (RANSAC - Random sample consensus) - Ideal Homography matrix calculated after 1000 iterations
4. Homography - Returns the homography matrix
5. Output - Shows the stitched images

# Image Mosaicing - Result

### Bakul Niwas - Four images to stitch

### Bakul Niwas - Stitched final image

### Taj Mahal - Six images to stitch

### Taj Mahal - Stitched final image



# Directory Structure
- ```src``` folder contains the source code. 
- ```images/Image Mosaicing/``` contains all the images to test the code on.
 
# Running the code
1. Run the jupyter notebook with all other directories present.
2. To stitch other images, modify the main.
