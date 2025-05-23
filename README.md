<div id="top">

<!-- HEADER STYLE: CLASSIC -->
<div align="center">


# FOOTBALL-ANALYSIS-SYSTEM

<em>Transforming Football Insights into Winning Strategies</em>

<!-- BADGES -->
<img src="https://img.shields.io/github/last-commit/amiliceviic/Football-Analysis-System?style=flat&logo=git&logoColor=white&color=0080ff" alt="last-commit">
<img src="https://img.shields.io/github/languages/top/amiliceviic/Football-Analysis-System?style=flat&color=0080ff" alt="repo-top-language">
<img src="https://img.shields.io/github/languages/count/amiliceviic/Football-Analysis-System?style=flat&color=0080ff" alt="repo-language-count">

<em>Built with the tools and technologies:</em>

<img src="https://img.shields.io/badge/Python-3776AB.svg?style=flat&logo=Python&logoColor=white" alt="Python">

</div>
<br>

---

## 📄 Table of Contents

- [Overview](#-overview)
- [Modules Used](#-modules-used)
- [Trained Models](#-trained-models)
- [Sample video](#-sample-video)
- [Requirements](#-requirements)
- [Getting Started](#-getting-started)
    - [Prerequisites](#-prerequisites)
    - [Installation](#-installation)
    - [Usage](#-usage)

---

## ✨ Overview

The objective of this project is to detect and track players, referees, and footballs within video footage by leveraging YOLO, a state-of-the-art AI object detection framework. The model was further enhanced through targeted training to improve accuracy.

Players are assigned to teams by applying K-means clustering on pixel data extracted from jersey colors, enabling effective team differentiation. This segmentation allows quantification of each team’s ball possession percentage during a match.

To accurately capture player movement, optical flow techniques are used to estimate camera motion between frames. This data is combined with perspective transformation to account for scene depth and perspective distortion, facilitating movement measurements in real-world units (meters) rather than pixels.

Finally, key player metrics such as speed and distance traveled on the field are calculated.

This comprehensive project integrates multiple advanced concepts and addresses practical challenges, making it an excellent example of applied machine learning for both novice and experienced practitioners.

![Screenshot](output_videos/screenshot.png)

**Why Football-Analysis-System?**

This project aims to enhance the analysis of football gameplay by providing robust tools for object detection and tracking. The core features include:

- 🎯 **Object Detection:** Utilizes a pre-trained YOLO model for accurate identification of players and the ball.
- 🏃 **Player and Ball Tracking:** Processes video frames to track movements, offering insights into gameplay dynamics.
- ⏱️ **Speed and Distance Estimation:** Calculates speed and distance for tracked objects, providing valuable performance metrics.
- 🎨 **Team Color Assignment:** Automatically assigns team colors to players, improving visual differentiation in analysis.
- 📷 **Camera Movement Estimation:** Analyzes camera motion to enhance tracking accuracy in dynamic environments.
- 📓 **User-Friendly Training Notebook:** Simplifies the training of YOLOv5 on custom datasets, making model training accessible to all developers.

---

## 🥡 Modules Used

The following modules are used in this project:
- YOLO: AI object detection model
- Kmeans: Pixel segmentation and clustering to detect t-shirt color
- Optical Flow: Measure camera movement
- Perspective Transformation: Represent scene depth and perspective
- Speed and distance calculation per player

---

## 🕹️ Trained Models

- [Trained Yolo v5](https://drive.google.com/file/d/1DC2kCygbBWUKheQ_9cFziCsYVSRw6axK/view?usp=sharing)

---

## ♟️ Sample video

-  [Sample input video](https://drive.google.com/file/d/1t6agoqggZKx6thamUuPAIdN_1zR9v9S_/view?usp=sharing)

---

## ✨ Requirements

To run this project, you need to have the following requirements installed:
- Python 3.x
- ultralytics
- supervision
- OpenCV
- NumPy
- Matplotlib
- Pandas

---

## 🚀 Getting Started

### 📋 Prerequisites

This project requires the following dependencies:

- **Programming Language:** Python
- **Package Manager:** Conda

### ⚙️ Installation

Build Football-Analysis-System from the source and intsall dependencies:

1. **Clone the repository:**

    ```sh
    ❯ git clone https://github.com/amiliceviic/Football-Analysis-System
    ```

2. **Navigate to the project directory:**

    ```sh
    ❯ cd Football-Analysis-System
    ```

3. **Install the dependencies:**

**Using [conda](https://docs.conda.io/):**

```sh
❯ conda env create -f conda.yml
```

### 💻 Usage

Run the project with:

**Using [conda](https://docs.conda.io/):**

```sh
conda activate {venv}
python {entrypoint}
```

```sh
conda activate {venv}
pytest
```

---

<div align="left"><a href="#top">⬆ Return</a></div>

---
