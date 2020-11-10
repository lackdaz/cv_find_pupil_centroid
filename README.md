# OpenCV Technical Interview Question

test_name: FindPupilCentroid

Authored by [Seth Loh](https://github.com/lackdaz) (c) 2020  
Telemedc Pte Ltd

## Objective

---
The human eye is one of the most common regions of interest on the human body, and is subject to a large body of literature and application use cases in eye-tracking and gaze estimation - [How does it work?](https://imotions.com/blog/eye-tracking-work/).

Your goal here is **develop a pupil detection algorithm to detect the centroid of the pupil** - usually the first step to any gaze-estimation algorithm. An embedded real-time solution would call for an image processing strategy that is lightweight and reliable. To illustrate, a camera running at 24 fps would require an execution of <41ms.

### Key Objectives  

1. Measure within 10 fps between frame computations.
1. Detect the centroid without jitter (defined as rapid changes in the centroid point between frames)  
1. Reject false centroids
1. Maintain a detection rate of 80%

### Must include  

1. Step-by-step intructions on how to install/run/deploy the program (README/markdown/.txt/). Choice of `python3-venv` or `docker`.
1. A written explanation of your image processing strategy.
1. Controls to pause/play the frame to facilitate review.
1. Clear annotation of centroid and pupil on frames.
1. A frame counting overlay.
1. Type-checked, [clean and refactored code](https://refactoring.guru/refactoring/smells). Any improper formatting will be **heavily penalised**.

### Bonus  

1. A double-frame view to help visualise the image processing layers.
1. Useful image annotations.
1. Argparse for other video filenames
1. Docstring explanations of code-blocks/functions.
1. Controls to yield next frame.
1. Dockerising the solution.

A sample frame capture could look something like:  
![sample_frame](https://github.com/lackdaz/find_pupil_centroid/blob/dev/assets/sample_frame.png)

**Note:** This is for illustrative purposes and **is not the model output**.

## Whitelisted libraries

1. python [standard libraries](https://docs.python.org/3/library/)
1. `python-opencv`
1. `numpy`
1. `imutils`

Contact your interviewer or file an issue if you wish to use any other libraries that are out of scope.

## Instructions

---

1. Fork or clone this library.
1. Download the dataset by running:  
`chmod +x get_videos.sh`  
and  
`get_videos.sh`  (MacOSX, Linux only  
or download from  
[https://tinyurl.com/tmc-cv2-challenge](https://tinyurl.com/tmc-cv2-challenge)
1. Create the `test_videos` directory if not created already, make sure the sample videos are located in here.
1. Provison your python virtual environment.
1. Create your entrypoint function at root and call it `pupil_detect.py`.
1. Develop, document and package your solution and contact your recruiter when ready.
1. You will be expectated to present your solution to a panel of interviewers.

## Asssesment Critera

---

1. Completion of key objectives [60%]
1. Code quality [20%]
1. Packaging [20%]
