# Computer Vision Projects

This repository contains five computer vision projects and computer assignments (CAs) developed as part of the **Fundamentals of Computer Vision** course at the University of Tehran.

Each project directory includes a `Description/` folder containing the official PDF specification and problem statements.

---

## Project Overview

| Project | Title / Focus | Primary Topics & Techniques | Detailed Guide |
| :--- | :--- | :--- | :--- |
| [**CA1**](./CA1/) | Image & Video Fundamentals, Color Spaces & Filtering | Color models (RGB, HSV, Grayscale), Histograms, Contrast Equalization, Spatial Filtering (Gaussian, Median, Sobel, Laplacian), Video Noise Reduction | Full explanation in [CA1.ipynb](./CA1/CA1.ipynb) |
| [**CA2**](./CA2/) | CAPTCHA Solving & Classical OCR Pipeline | Denoising, Deblurring, Morphological Operations, Character Segmentation, Template Matching & Classical OCR (without ML) | Full explanation in [CA2.ipynb](./CA2/CA2.ipynb) |
| [**CA3**](./CA3/) | Pre-trained Vision Models & Autoencoders | Pre-trained CNNs for Face & Gender/Age Detection, Haar Cascades / YOLO for Cat Detection, Convolutional Autoencoder for Grayscale Image Colorization | Full explanation in [Cat_Detection.ipynb](./CA3/Cat_Detection.ipynb), [Face_Detection.ipynb](./CA3/Face_Detection.ipynb), & [Q3.ipynb](./CA3/Q3.ipynb) |
| [**CA4**](./CA4/) | Deep Learning Image Classification on Intel Dataset | Convolutional Neural Networks (CNNs), Data Augmentation, Regularization (Dropout, BatchNorm), Overfitting Analysis, Hyperparameter Tuning | Full explanation in [CV_HW4_CNN_Colab.ipynb](./CA4/CV_HW4_CNN_Colab.ipynb) |
| [**Final Project**](./Final Project/) | Old Photo Restoration & Enhancement | Deep U-Net Architecture, Image Denoising, Scratch/Artifact Inpainting, Super-Resolution, Quantitative (PSNR, SSIM) & Qualitative Evaluation, Gradio UI | Full explanation in [CV_FinalProject_810101400_810102303.ipynb](./Final%20Project/CV_FinalProject_810101400_810102303.ipynb) |

---

## Detailed Project Descriptions

### 1. [CA1: Fundamentals of Image and Video Processing](./CA1/)
* **Description PDF:** [CV_HW1.pdf](./CA1/Description/CV_HW1.pdf)
* **Full Implementation:** [CA1.ipynb](./CA1/CA1.ipynb)
* **Summary:**
  * **Color Spaces & Manipulations:** Exploration of RGB, Grayscale, Binary, and HSV color models, channel decomposition, and hue/saturation/value alterations.
  * **Histogram & Contrast Enhancement:** Contrast computation, image histogram visualization, histogram stretching, and histogram equalization.
  * **Noise & Spatial Filtering:** Simulating Gaussian and Salt-and-Pepper noise; designing custom convolutional 2D filters for low-pass smoothing (Mean, Gaussian) and high-pass edge detection (Sobel, Prewitt, Laplacian), and comparing them with OpenCV built-ins.
  * **Video Processing:** Extracting video frames, introducing dynamic noise, and applying frame-by-frame temporal/spatial filtering (Median filter) to restore video quality.

---

### 2. [CA2: CAPTCHA Recognition via Classical Image Processing](./CA2/)
* **Description PDF:** [CV_HW2.pdf](./CA2/Description/CV_HW2.pdf)
* **Full Implementation:** [CA2.ipynb](./CA2/CA2.ipynb)
* **Summary:**
  * **Image Preprocessing:** Deblurring and noise reduction on synthetic CAPTCHA images containing alphanumeric characters.
  * **Segmentation:** Binarization, morphological transformations (dilation, erosion, opening, closing), contour analysis, and bounding-box extraction to isolate individual characters.
  * **Character Recognition (OCR):** Developing a classical template matching and metric comparison pipeline without modern machine learning models, benchmarked across noisy character sets.

---

### 3. [CA3: Pre-trained Deep Learning Models & Image Colorization](./CA3/)
* **Description PDF:** [CV_HW3.pdf](./CA3/Description/CV_HW3.pdf)
* **Full Implementations:**
  * Face, Age & Gender Detection: [Face_Detection.ipynb](./CA3/Face_Detection.ipynb)
  * Cat Detection: [Cat_Detection.ipynb](./CA3/Cat_Detection.ipynb)
  * Image Colorization Autoencoder: [Q3.ipynb](./CA3/Q3.ipynb)
* **Summary:**
  * **Face, Age & Gender Classification:** Utilizing deep Caffe/OpenCV pre-trained models to detect human faces in video streams and predict age brackets and gender with confidence scores.
  * **Cat Detection:** Implementing object detection pipelines to localize cats within images/videos using pre-trained detectors.
  * **Deep Image Colorization:** Designing and training an autoencoder network in Keras/TensorFlow to predict chrominance ($a^*, b^*$) channels from luminance ($L$) inputs, transforming grayscale photographs into plausible colored images.

---

### 4. [CA4: Natural Image Classification with CNNs](./CA4/)
* **Description PDF:** [CV-HW4.pdf](./CA4/Description/CV-HW4.pdf)
* **Full Implementation:** [CV_HW4_CNN_Colab.ipynb](./CA4/CV_HW4_CNN_Colab.ipynb)
* **Summary:**
  * **Dataset:** Intel Image Classification dataset covering 6 natural scene classes: *buildings, forest, glacier, mountain, sea, street*.
  * **Architecture Design:** Constructing convolutional neural network architectures with Conv2D, MaxPooling, Batch Normalization, and Dropout layers.
  * **Training & Optimization:** End-to-end training pipeline using Sparse Categorical Crossentropy, Adam optimizer, learning rate schedules, and data augmentation.
  * **Diagnostics & Evaluation:** Plotting training vs. validation accuracy/loss curves, diagnosing underfitting and overfitting behaviors, and computing confusion matrices.

---

### 5. [Final Project: Old Photo Restoration & Enhancement](./Final%20Project/)
* **Description PDF:** [CV-Final Project.pdf](./Final%20Project/Description/CV-Final%20Project.pdf)
* **Full Implementation:** [CV_FinalProject_810101400_810102303.ipynb](./Final%20Project/CV_FinalProject_810101400_810102303.ipynb)
* **Summary:**
  * **End-to-End Image Restoration:** Restoration of aged, degraded, scratched, and noisy photographs using deep learning.
  * **U-Net Architecture:** Implementing a multi-scale U-Net with skip connections to reconstruct lost spatial high-frequency details.
  * **Metrics & Benchmarking:** Quantitative evaluation using Peak Signal-to-Noise Ratio (PSNR) and Structural Similarity Index (SSIM), coupled with qualitative visual inspection.
  * **Interactive Deployment:** An interactive web demo built with Gradio allowing users to upload damaged photos and view real-time restoration comparisons.

