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
<p float="left">
  <img src="https://user-images.githubusercontent.com/44245211/137888046-549ea5dd-1fad-4879-8f2d-7ffa4bf52e30.jpg" width="220" />
  <img src="https://user-images.githubusercontent.com/44245211/137888053-96b94447-74ca-414d-a4c0-4a9939020255.jpg" width="220" /> 
  <img src="https://user-images.githubusercontent.com/44245211/137888058-667aacff-880b-41c4-8ef8-df81ee9d7bd0.jpg" width="220" /> 
  <img src="https://user-images.githubusercontent.com/44245211/137888061-8c832609-d43e-4998-ac35-deba5c8a7c08.jpg" width="220" />
</p>

### Bakul Niwas - Stitched final image

### Taj Mahal - Six images to stitch

### Taj Mahal - Stitched final image



# Directory Structure
- ```src``` folder contains the source code. 
- ```images/Image Mosaicing/``` contains all the images to test the code on.
 
# Running the code
1. Run the jupyter notebook with all other directories present.
2. To stitch other images, modify the main.
