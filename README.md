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
  <img src="https://user-images.githubusercontent.com/44245211/137888046-549ea5dd-1fad-4879-8f2d-7ffa4bf52e30.jpg" width="200" />
  <img src="https://user-images.githubusercontent.com/44245211/137888053-96b94447-74ca-414d-a4c0-4a9939020255.jpg" width="200" /> 
  <img src="https://user-images.githubusercontent.com/44245211/137888058-667aacff-880b-41c4-8ef8-df81ee9d7bd0.jpg" width="200" /> 
  <img src="https://user-images.githubusercontent.com/44245211/137888061-8c832609-d43e-4998-ac35-deba5c8a7c08.jpg" width="200" />
</p>

### Bakul Niwas - Stitched final image
<p float="left">
  <img src="https://user-images.githubusercontent.com/44245211/137891874-c2d84fff-dcdf-45e5-8bb4-d01f029ae674.png" width="895" />
</p>


### Taj Mahal - Six images to stitch
<p align="left">
  <img src="https://user-images.githubusercontent.com/44245211/137892466-ad04abd6-4e78-4263-9e47-6c67463e2426.png" width="200" />
  <img src="https://user-images.githubusercontent.com/44245211/137892481-63764503-9103-4823-af1c-a9d5a8fa7170.png" width="200" />
  <img src="https://user-images.githubusercontent.com/44245211/137892483-081300c7-dd8a-4878-8e07-ac521d6529ad.png" width="200" />
</p>

<p align="left">
  <img src="https://user-images.githubusercontent.com/44245211/137892484-a0c39339-8cd5-4cc6-8ea0-5dc677d0a147.png" width="200" />
  <img src="https://user-images.githubusercontent.com/44245211/137892485-730d44f8-509a-4a27-9078-b5932d0e041b.png" width="200" />
  <img src="https://user-images.githubusercontent.com/44245211/137893025-3c02fbc7-15b6-4ecd-9a65-0e10f7128e35.png" width="200" />
</p>

### Taj Mahal - Stitched final image
<p float="left">
  <img src="https://user-images.githubusercontent.com/44245211/137891993-1fd13839-5a18-41f8-8b1a-e79ca39f127f.png" width="895" />
</p>

### Himalaya Block - Four images to stitch
<p align="left">
  <img src="https://user-images.githubusercontent.com/44245211/137893541-4931f3ac-f9e4-42fe-a3a1-c2085c1b9e15.jpg" width="200" />
  <img src="https://user-images.githubusercontent.com/44245211/137893560-2a35091d-b21b-4e99-9f41-77756d2b09d9.jpg" width="200" />
  <img src="https://user-images.githubusercontent.com/44245211/137893564-ef647fa8-07ee-4a61-8f09-c6f1afbdbbff.jpg" width="200" />
  <img src="https://user-images.githubusercontent.com/44245211/137893567-234710c1-646c-4da8-b2ea-8a83c3bf225c.jpg" width="200" />
</p>

### Himalaya Block - Stitched final image

<p float="left">
  <img src="https://user-images.githubusercontent.com/44245211/137893757-abf2cdca-890f-442d-8325-2ee5ec429561.png" width="834" />
</p>

# Directory Structure
- ```src``` folder contains the source code. 
- ```images/Image Mosaicing/``` contains all the images to test the code on.
 
# Running the code
1. Run the jupyter notebook with all other directories present.
2. To stitch other images, modify the main.
