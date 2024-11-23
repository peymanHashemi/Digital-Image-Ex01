# Digital Image Processing (DIP) Exercises
Exercises for Digital Image Processing Course - Amirkabir University of Technology Spring 2022

By Peyman Hashemi Spring/Summer 2022

# Content
- Table of Contents
  * [EX1](#Exercise-1) [Face Symmetry, Climate Change, Steganography, Pacman with OpenCV]
  * [EX2](#Exercise-2) [Pedestrian/Motion Detection, Bilateral Filtering Poster, Seam Carving]
  * [EX3](#Exercise-3) [Fourier Analysis, Hybrid Image Generation with frequency separation]
  * [EX4](#Exercise-4) [Image Restoration, Perspective Transform, Face Morphing with Delaunay Triangulation]
  * [EX5](#Exercise-5) [Image Compression, Image Filtering, Obejct Detection with Morphological techniques]

# Exercise 1


# Question 1
Is beauty measurable?
In this exercise we have some pictures of famouse soccer players (Dataset1). We try to measure beauty with PSNR and SSIM metric.
At first we create a mirror of every image and we split original and mirrored image and we combine them in ‘L ⅃’, ‘Я R’, and ‘Я ⅃’ order.
At last compute PSNR and SSIM metrics for every combined picture.

Result : 

<img src="https://user-images.githubusercontent.com/62074677/214143563-73d5f1ea-a9fa-4e75-b667-3fe51e52421b.png" width=20% height=20%> <img src="https://user-images.githubusercontent.com/62074677/214143265-b3a99280-f193-4837-bd31-eb09194305b0.png" width=20% height=20%> <img src="https://user-images.githubusercontent.com/62074677/214143330-0ed1f746-0e00-4cd1-8b41-6b59d0da8b09.png" width=20% height=20%> <img src="https://user-images.githubusercontent.com/62074677/214143371-ba2f6f5d-5bcb-4d00-943c-8f6446380400.png" width=20% height=20%>

# Question 2
The Art of Hiding Messages in Pixels
We are given two seemingly random grayscale images which contain a secret message. 
The idea is to move one image on another and find the hidden message using basic image operations.

Result :

<img src="https://user-images.githubusercontent.com/62074677/214144155-cb10d759-36dd-44f3-a278-cff062cbab66.png" width=30% height=30%>

# Question 3
Analyzing Some Global Warming Impacts
We are given 4 set of datasets.

A) We should find the approximate volume of water evaporated between 2 images.

B) We should find the approximate volume of water evaporated.

C) what proportion of the glacier has been melted over the given time interval?

D) We should plot a bar graph representing the approximate volume of the lake in each five years separately.


Result (C):

<img src="https://user-images.githubusercontent.com/62074677/214143724-7f4f4741-204e-40c5-a556-0c63fbf8ae68.jpg" width=30% height=30%>  <img src="https://user-images.githubusercontent.com/62074677/214143695-af37895c-23e2-4164-b132-1cfd63e64701.jpg" width=30% height=30%>

<img src="https://user-images.githubusercontent.com/62074677/214143788-360ec5c8-5699-4b70-b8f7-6aea09d3aa90.png" width=30% height=30%>  <img src="https://user-images.githubusercontent.com/62074677/214143762-da1a5e83-8204-465e-b651-83dc36c45651.png" width=30% height=30%>

# Question 4
 Creating A Pac-Man Demo
 
In this problem, the goal is to create a demo version of Pac-Man, 
which, in spite of being non-playable, follows the rules of the game.
You are given an image of the maze at its initial point as well as different elements of the game in various states.
 
Result :

<img src="https://user-images.githubusercontent.com/62074677/214148368-eda6bb30-5b56-4d35-be76-4f21acd98f8c.gif">


# Exercise 2
Exercises for Digital Image Processing Course - Spring 2022

By Peyman Hashemi

## Question 1: Image Point Processing
We explore various image point processing techniques. These include image negation, bit-plane slicing, histogram computation, and equalization. The exercise also involves applying thresholding and scaling operations. Finally, the task ends with histogram specification for intensity transformation.
Results: The answer is provided in following PDF


#ImageNegative #HistogramEqualization #BitPlaneSlicing
## Question 2: Motion Detection Using Bit-plane Slicing
We slice grayscale images into bit-planes and compare consecutive frames using the XOR function to detect motion. The motion is highlighted by reconstructing the image from the significant bit-planes.
Results:

<img style="width:200px" src="https://github.com/user-attachments/assets/09c1409a-5777-40fd-b5cf-12b3779d5a8c" >


<img style="width:200px" src="https://github.com/user-attachments/assets/193f2b0e-f919-4d16-b46f-466f0c7eba34" >


<img style="width:200px" src="https://github.com/user-attachments/assets/ab8a44e2-9883-4fce-8ee3-d7fe3fe6e04f" >


#MotionDetection #BitPlaneXOR #FootballPlayerTracking

# Question 3: Pedestrian Detection
We apply image averaging and thresholding to detect pedestrians in video frames. The background is estimated using multiple frames and subtracted from the foreground to count individuals in test frames.
Results:

<img style="width:300px" src="https://github.com/user-attachments/assets/808e47db-bf23-4592-a0c4-bde7ce675627">


<img style="width:300px" src="https://github.com/user-attachments/assets/961ea9de-d1f5-4daa-a20e-5a5e4ffe4715">


<img style="width:300px" src="https://github.com/user-attachments/assets/d1e9987f-8868-4fd5-9411-1d830bb88af6">


<img style="width:600px" src="https://github.com/user-attachments/assets/8dfee085-d998-4626-9b5f-61b720933c91">

#PedestrianDetection #ImageAveraging #ForegroundExtraction

## Question 4: Image Obamafication
Inspired by the iconic "Hope" poster, this exercise applies bilateral filtering and color mapping based on intensity thresholds to create a stylized effect.
Results: 



<img src="https://github.com/user-attachments/assets/07f669fc-124c-4a0d-a303-9c2c7b1689ed" width=30% height=30%>
<br>
<img src="https://github.com/user-attachments/assets/0c700d18-e093-4ff5-94be-625e3fbf10fe" width=30% height=30%>

#BilateralFiltering #ColorMapping #Posterization
## Question 5: Seam Carving for Image Resizing
We use seam carving to resize images without distorting important content. The technique involves finding and removing low-energy pixel paths, reducing image dimensions while preserving key features.
Results:

<img src="https://github.com/user-attachments/assets/54229444-2304-48cd-a7ef-ca8d45f2f9f0">

#SeamCarving #ImageResizing #DynamicProgramming

## Question 6: Explanatory Questions
A set of theoretical questions regarding spatial filters, noise reduction, and template matching were explored.
Results: The answer is provided in following PDF

#ImageFiltering #NoiseReduction #TemplateMatching

# Exercise 3

## Question 1: Fundamentals of Fourier Transform (I)

This section explores the foundational concepts of Fourier Transform, including Discrete Cosine Transform (DCT), Discrete Fourier Transform (DFT), and Sampling Theorem. The tasks include:

- Calculating the DC coefficient and understanding its significance.
- Proving relationships between Fourier basis functions and image patterns.
- Understanding the impact of sampling distance and aliasing.
#FourierTransform #SamplingTheorem #ImageFrequencyAnalysis

---

## Question 2: Fundamentals of Fourier Transform (II) - 2D Convolution

The second section applies Fourier analysis to 2D Convolution. Key tasks include:

- Deriving equivalent filters in the frequency domain.
- Identifying low-pass and high-pass filters through mathematical proofs.
- Understanding the effects of filter transformations, such as band-pass and notch filters, on images.
#2DConvolution #FrequencyDomainFilters #ImageFiltering

---

## Question 3: Fourier Analysis in the Spatial and Frequency Domains

This question focuses on analyzing images using Fourier Transforms in both spatial and frequency domains. The tasks include:

- Matching patterns in images to their Fourier magnitude representations.
- Exploring how structures in the spatial domain correspond to frequency domain features.

Results:

<img style="width:600px" src="https://github.com/user-attachments/assets/42464821-c9a8-4784-be67-a95e153764fa">
<br>
<img style="width:600px" src="https://github.com/user-attachments/assets/b22af1b7-8c9d-4282-8568-3f0e7dbbcdda">

#FourierAnalysis #SpatialVsFrequencyDomain #PatternRecognition

---

## Question 4: Color Assimilation Grid Illusion and Munker’s Illusion

We analyze perceptual illusions using Fourier Transform and filtering techniques:

- Proving the "Color Assimilation Grid Illusion" by analyzing grid lines in various color spaces (e.g., RGB, HSV, YCbCr, Lab).
- Removing grid patterns and restoring grayscale images using band-pass filters.
- Verifying the uniformity of shapes in Munker’s Illusion despite apparent color differences.

Results:

<img style="width:600px" src="https://github.com/user-attachments/assets/f33e756e-2ee3-4f6d-8563-23753d9c0873">
<br>
<img style="width:600px" src="https://github.com/user-attachments/assets/f83a5fd0-3d5f-455b-abe6-8e3d9ba84a1c">
<br>
#ColorIllusion #FourierFiltering #MunkersIllusion

---

## Question 5: Hybrid Images – Merging Frequency Components

This exercise demonstrates how to create hybrid images by combining high-frequency details of one image with the low-frequency content of another. The tasks include:

- Aligning image pairs to ensure meaningful hybrid results.
- Applying low-pass and high-pass filters with appropriate cut-off frequencies.
- Visualizing the hybridization process with progressively filtered outputs.

Results:

<img style="width:600px" src="https://github.com/user-attachments/assets/1adb0ae7-5c0e-4193-be53-2ba97759ded0"> <br> <img style="width:600px" src="https://github.com/user-attachments/assets/77a60275-4faf-47b3-897f-4ed360e76233"> <br> <img style="width:600px" src="https://github.com/user-attachments/assets/f03f50d4-8be2-40c6-bfc3-0185316c0d46"> <br> <img style="width:600px" src="https://github.com/user-attachments/assets/9ffd6969-7302-419b-a8ee-4f2d6e3279a7">

#HybridImages #HighLowFrequency #VisualPerception

---


# Exercise 4

## Question 1: The Magnificent Eleven - Restoring Historical Photos

This question involves restoring degraded historical photographs from the D-Day landings, known as "The Magnificent Eleven." The tasks include:

- **Step 1**: Computing the Fourier Transform to identify vertical and horizontal noise patterns.
- **Step 2**: Removing these patterns using filters and sharpening techniques (e.g., applying specific kernels).
- **Step 3**: Applying normalization and advanced denoising methods like bilateral filtering and `fastNlMeansDenoising`.
- **Step 4**: Sharpening the image post-denoising for improved visual clarity.

### Results:

<img style="width:500px" src="https://github.com/user-attachments/assets/df451ba6-4082-4ffb-8731-8305bb462a13">
<br>
<img style="width:500px" src="https://github.com/user-attachments/assets/9a3c100d-2a8f-4217-a93b-d923ebc87ba0">

#ImageRestoration #Denoising #WWIIHistory

---

## Question 2: Wait for Me, Daddy - Resolution Enhancement

This question focuses on enhancing the resolution of the iconic Canadian photograph *"Wait for Me, Daddy"* through interpolation methods. The steps include:

- **a. Nearest-Neighbor Interpolation**: Resizing the image using the nearest-pixel value.
- **b. Bilinear Interpolation**: Smoothing transitions using weighted averages of neighboring pixels.
- **c. Nearest Neighbor Value Interpolation**: Estimating missing pixel values based on nearest neighbors.
- **d. Non-Uniform Interpolation**: Resampling multiple low-resolution images with subpixel shifts to create a higher-resolution image.
- **e. PSNR Calculation**: Evaluating and comparing results of all methods using the PSNR metric.

### Results:

<img style="width:500px" src="https://github.com/user-attachments/assets/ebfa00b2-1618-49b5-9006-1dd25f6c67b7">
<br>
#ResolutionEnhancement #ImageInterpolation #PSNREvaluation

---

## Question 3: Sonderkommando Photographs - Recovering Evidence

This question involves restoring rare and historically significant photographs from Auschwitz, taken secretly by prisoners. The tasks include:

- **a. Geometric Transformation**: Aligning the images into a proper frame for further processing.
- **b. Image Restoration**: Applying filters and enhancement techniques to improve the visual quality.
- **c. Final Denoising and Sharpening**: Using advanced methods to remove artifacts and improve clarity.

### Results:
<img style="width:500px" src="https://github.com/user-attachments/assets/54b3f27e-3420-48a7-af83-398f4b4316cc">
<br>
<img style="width:500px" src="https://github.com/user-attachments/assets/e82b9078-56a8-49fc-8808-5953e6a93a3b">


#ImageRestoration #AuschwitzPhotos #GeometricTransformation

---

## Question 4: Morphing a Soldier’s Face - Before and After WWII

This question demonstrates morphing techniques to visualize changes in the appearance of a WWII soldier before and after the war. The tasks include:

- **a. Naïve Method**: Interpolating between the images pixel-by-pixel, producing 10 intermediate images.
- **b. Keypoint Detection**: Manually identifying facial features and prominent points for accurate alignment.
- **c. Delaunay Triangulation**: Dividing the face into triangles for localized transformations.
- **d. Affine Transformation**: Morphing corresponding triangles between images and generating intermediate frames.
- **e. Animation**: Creating a two-second video with 61 frames to visualize the transition.

### Results:

<img style="width:500px" src="https://github.com/user-attachments/assets/14d2c6c8-ee06-42a4-8dc6-07e5a4252b4d">
<br>
<img style="width:700px" src="https://github.com/user-attachments/assets/77f6b434-3744-491c-b972-201a3db72a23">

#ImageMorphing #FacialTransformation #WWIIImpacts

---


# Exercise 5

### Question 1: Image Compression Using Run-Length and Huffman Coding
We explore fundamental image compression techniques, starting with run-length encoding and zig-zag ordering for binary images. Huffman coding is then applied to generate efficient codebooks based on symbol probabilities. The tasks also include entropy comparison, bit-rate calculation, and compression ratio analysis.

### Steps:
1. Convert the image to binary and calculate run-length encoding.
2. Apply zig-zag ordering to arrange the pixel sequence.
3. Generate Huffman codes for each symbol and calculate entropy and compression metrics.

#ImageCompression #RunLengthCoding #HuffmanEncoding

---

### Question 2: JPEG Compression and Quantization
This task focuses on lossy compression with JPEG-like quantization. Starting with 4×4 DCT coefficients, quantization is applied, followed by vectorization and run-length encoding. Spatially neighboring blocks are analyzed for further compression.

1. Quantize 4×4 DCT coefficients using a given quantization matrix.
2. Order coefficients with zig-zag traversal and encode using run-length encoding.
3. Propose additional compression techniques for neighboring blocks.

### Results:

<img style="width:700px" src="https://github.com/user-attachments/assets/012ade74-027a-4647-bbf7-dbb9c5207403"> <br>
<img style="width:400px" src="https://github.com/user-attachments/assets/bcdd23e3-f020-4d04-b8a6-afcec04b7101">
<img style="width:400px" src="https://github.com/user-attachments/assets/8442c040-37c4-4b9a-ae0c-fb65b8c6266d">
<img style="width:400px" src="https://github.com/user-attachments/assets/caebdf92-115f-4daf-8557-2f20364ff3ea">

#JPEGCompression #Quantization #RunLengthEncoding

---

### Question 3: Morphological Edge Detection
Morphological operations such as dilation, erosion, opening, and closing are applied to detect edges in grayscale images. Each approach is compared for accuracy in edge preservation and noise reduction.

### Steps:
1. Apply second-order derivatives with dilation and erosion.
2. Perform edge detection using combinations of opening and closing.
3. Compare outputs for clarity and noise resilience.

### Results:
<img style="width:600px" src="https://github.com/user-attachments/assets/2b1bf62f-141b-48e0-bc87-7b62a76baa1a">
<img style="width:600px" src="https://github.com/user-attachments/assets/4d73b1e2-21fa-4e3f-ad9e-fd42df4d34ba">
<img style="width:600px" src="https://github.com/user-attachments/assets/24eaf03c-d877-479d-93e5-b36d26ceeed9">


### Final result of Object Detection and Counting:
### Steps:
1. Remove the background using morphological operators like opening and closing.
2. Count and categorize items using boundary detection and connected component analysis.
3. Calculate the total cost based on item categories.
<img style="width:600px" src="https://github.com/user-attachments/assets/c1a0e514-1132-4aa4-8164-d9bea95a6335">

#Morphology #EdgeDetection #ImageFiltering

---


