# Content
- Table of Contents
  * [EX1](#Digital Image Processing - Exercise 1) [Face Symmetry, Climate Change, Steganography, Pacman with OpenCV]
  * [EX2](#Digital Image Processing - Exercise 2) [Pedestrian/Motion Detection, Bilateral Filtering Poster, Seam Carving]
  * [EX3](#EX3) [Fourier Analysis, Hybrid Image Generation with frequency separation]
  * [EX4](#EX4) [Image Restoration, Perspective Transform, Face Morphing with Delaunay Triangulation]
  * [EX5](#EX5) [Image Compression, Image Filtering, Obejct Detection with Morphological techniques]

# Digital Image Processing - Exercise 1
Exercises for Digital Image Processing Course - Amirkabir University of Technology Spring 2022

By Peyman Hashemi Spring/Summer 2022

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


# Digital Image Processing - Exercise 2
Exercises for Digital Image Processing Course - Spring 2022

By Peyman Hashemi

## Question 1: Image Point Processing
We explore various image point processing techniques. These include image negation, bit-plane slicing, histogram computation, and equalization. The exercise also involves applying thresholding and scaling operations. Finally, the task ends with histogram specification for intensity transformation.
Results: The answer is provided in following PDF


#ImageNegative #HistogramEqualization #BitPlaneSlicing
## Question 2: Motion Detection Using Bit-plane Slicing
We slice grayscale images into bit-planes and compare consecutive frames using the XOR function to detect motion. The motion is highlighted by reconstructing the image from the significant bit-planes.
Results:

<img src="https://github.com/user-attachments/assets/09c1409a-5777-40fd-b5cf-12b3779d5a8c" width=20% height=20%>
<img src="https://github.com/user-attachments/assets/193f2b0e-f919-4d16-b46f-466f0c7eba34" width=20% height=20%>
<img src="https://github.com/user-attachments/assets/ab8a44e2-9883-4fce-8ee3-d7fe3fe6e04f" width=20% height=20%>

#MotionDetection #BitPlaneXOR #FootballPlayerTracking
# Question 3: Pedestrian Detection
We apply image averaging and thresholding to detect pedestrians in video frames. The background is estimated using multiple frames and subtracted from the foreground to count individuals in test frames.
Results:

<img src="https://github.com/user-attachments/assets/808e47db-bf23-4592-a0c4-bde7ce675627" width=20% height=20%>
<img src="https://github.com/user-attachments/assets/961ea9de-d1f5-4daa-a20e-5a5e4ffe4715" width=20% height=20%>
<img src="https://github.com/user-attachments/assets/d1e9987f-8868-4fd5-9411-1d830bb88af6" width=20% height=20%>

#PedestrianDetection #ImageAveraging #ForegroundExtraction
## Question 4: Image Obamafication
Inspired by the iconic "Hope" poster, this exercise applies bilateral filtering and color mapping based on intensity thresholds to create a stylized effect.
Results: 

<img src="https://github.com/user-attachments/assets/bde9695f-63ed-48ee-a760-66e7d8ebd2dd" width=20% height=20%>
<img src="https://github.com/user-attachments/assets/2f4f4795-83be-4f7f-b819-70977ad11a61" width=20% height=20%>

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
