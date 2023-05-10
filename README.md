<a name="readme-top"></a>

<!-- PROJECT LOGO -->
<br />
<div align="center">
  <h3 align="center">Mediapipe Object Detection Python Exapmles</h3>

  <p align="center">
    Python jupyter notebook examples using several <a href="https://developers.google.com/mediapipe">Mediapipe</a> solutions with opencv for live webcam detection.
    <br />
    <br />
  </p>
</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#contact">Contact</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

The [Mediapipe documentation](https://developers.google.com/mediapipe) has several examples for still image detection with python, but the live stream python examples were not fully implemented. This repo contains a few implementations that demonstrate live stream functionality of the following solutions / APIs:

* [Object Detection](https://developers.google.com/mediapipe/solutions/vision/object_detector/python)
* [Gesture Recognition](https://developers.google.com/mediapipe/solutions/vision/gesture_recognizer/python)
* [Holistic landmark detection](https://developers.google.com/mediapipe/solutions/vision/holistic_landmarker)
* [Face Mesh](https://developers.google.com/mediapipe/solutions/vision/face_landmarker)

Since much of the example documentation in the Medipipe docs didn't include full implemntation examples, these represent the results of my exploration.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- GETTING STARTED -->
## Getting Started

To get a local copy up and running follow these simple example steps.

### Prerequisites

An install of [Python 3.9](https://www.python.org/downloads/release/python-3916/), either from python.org, [conda](https://docs.conda.io/en/latest/miniconda.html), or your preferred method.

* If you want to run the [gesture recognizer]() you will need a [pre-trained model](https://storage.googleapis.com/mediapipe-tasks/gesture_recognizer/gesture_recognizer.task).
* If you want to run the [object detector]() you will need a [pre-trained model](https://developers.google.com/mediapipe/solutions/vision/object_detector/index#models).

### Installation

_Below is an example of how you can instruct your audience on installing and setting up your app. This template doesn't rely on any external dependencies or services._
1. Clone the repo
  ```sh
  cd /folder/where/you/want/the/copy
  git clone https://github.com/rdarneal/mediapipe_python_examples.git
  ```
2. Install packages, either via python or conda:
  * python
    ```sh
    python -m pip install requirements.txt
    ```
  * conda
    ```sh
    conda env create -n myenv -f environment.yml
    ```
3. Add the pre-trained models to your project folder :
  * Gesture Recognition model
  ```sh
  wget https://storage.googleapis.com/mediapipe-tasks/gesture_recognizer/gesture_recognizer.task
  ```
  * Object detector model (other options are available [here](https://developers.google.com/mediapipe/solutions/vision/object_detector/index#models))
  ```sh
  wget -O efficientdet.tflite https://storage.googleapis.com/mediapipe-tasks/object_detector/efficientdet_lite0_uint8.tflite
  ```
4. Open the file in VSCode, Jupyter, or your favorite IDE:
  ```sh
  # VSCode example
  code .
  ```

5. Run the jupyter notesbook. Refer to information and instructions in the cells.

<!-- USAGE EXAMPLES -->
## Usage

After following the installation instructions, you can open the `ipynb` files and run all cells to start up a live-stream webcam detection.
* `face_mesh_live`: Mediapipe face mesh API example notebook
* `gesture_recognition`: Mediapipe gesture recognition live stream example notebook
* `holistic_model`: Mediapipe holistic model live stream example notebook
* `object_detection`: Mediapipe livestream object detection example notebook

_For more examples, or for working with still images or pre-recorded video, check out Mediapipe's [Documentation](https://developers.google.com/mediapipe)_

<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- CONTACT -->
## Contact

Robert Darneal- [@rdarneal](https://github.com/rdarneal)

Project Link: [https://github.com/rdarneal/mediapipe_python_examples](https://github.com/rdarneal/mediapipe_python_examples)

<p align="right">(<a href="#readme-top">back to top</a>)</p>
