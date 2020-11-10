# find_pupil_centroid

OpenCV Technical Interview Question  
Authored by Seth Loh (c) 2020  
Telemedc Pte Ltd

## Objectives

---
The human eye is one of the most common regions of interest on the human body, and is subject to a large body of literature and application use cases in eye-tracking and gaze estimation - [How does it work?](https://imotions.com/blog/eye-tracking-work/).

Your goal here is **develop a pupil detection algorithm to detect the centroid of the pupil** - usually the first step to any gaze-estimation algorithm. An embedded real-time solution would call for an image processing strategy that is lightweight and reliable. To illustrate, a camera running at 24 fps would require an execution of <41ms.

### Key Objectives  

1. Measure within 15 fps between frame computations.
1. Detect the centroid without jitter (defined as rapid changes in the centroid point between frames)  
1. Reject false centroids
1. Maintain a detection rate of 80%

### Must include  

1. Step-by-step intructions on how to run/deploy the program (README/markdown/.txt/)
1. A written explanation of your image processing strategy
1. A utility to pause/play the frame to facilitate review.
1. Type-checked, [clean and refactored code](https://refactoring.guru/refactoring/smells). Any improper formatting will be **heavily penalised**.

### Bonus  

1. Dockerize / package your solution.
1. A double-frame view to help visualise the image processing layers.

## Video Samples

---

1. Download the dataset by running:
`get_videos.sh` (MacOSX, Linux only) or  
[https://tinyurl.com/tmc-cv2-challenge](https://tinyurl.com/tmc-cv2-challenge)
