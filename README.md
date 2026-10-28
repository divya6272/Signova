#  Signova – Two-Way Indian Sign Language Communication System

Signova is a deep learning–based Indian Sign Language (ISL) recognition system designed to bridge the communication gap between deaf and hearing individuals.

The system supports two-way communication by converting:

- ✋ **Hand Gestures → Text**
- ⌨️ **Text → ISL GIFs**

This project is a research-driven prototype focused on simplicity, real-time performance, and accessibility using a standard webcam.

##  Problem Statement

Many deaf and hard-of-hearing people use sign language to communicate. However, communication barriers arise when others do not understand sign language, particularly in:

- Daily conversations
- Healthcare
- Education
- Social interactions

Signova explores a camera-based approach to sign language recognition without requiring specialized sensors or wearable devices.

##  Objectives

- Enable real-time ISL gesture recognition.
- Support two-way communication.
- Avoid external sensors and gloves.
- Use low-cost, camera-based vision.
- Explore accessible sign language communication.

##  System Overview

The system follows these stages:

1. Webcam captures hand gesture images.
2. Images are preprocessed, including resizing and normalization.
3. A Convolutional Neural Network (CNN) extracts relevant visual features.
4. The model classifies the hand gesture.
5. The system displays the corresponding text.

For text-to-sign communication, the system displays corresponding ISL GIFs.

### Communication Workflow

**Gesture → Image Processing → CNN Classification → Text**

**Text → Gesture Mapping → ISL GIF**

##  Dataset Details

A custom Indian Sign Language hand gesture dataset was created specifically for the Signova project.

| Attribute | Description |
|---|---|
| Dataset Type | Custom ISL hand gesture image dataset |
| Total Gesture Classes | 12 |
| Images per Gesture | Approximately 250 |
| Total Images | Approximately 3,000 |
| Capture Device | Webcam |
| Variations | Lighting, background, and hand pose |

### Supported Gestures

The dataset contains images for the following 12 gesture classes:

1. Hello
2. Namaste
3. Help
4. Doctor
5. Food
6. Water
7. Yes
8. No
9. Please
10. Stop
11. Thank You
12. Friends

###  Download Dataset

The complete dataset is available as a ZIP file in the GitHub Releases section.

**[Download Signova Hand Gesture Dataset](https://github.com/divya6272/Signova/releases)**

The dataset is shared to encourage learning, experimentation, and further development of sign language recognition systems.

###  Dataset License

The Signova hand gesture dataset is intended to be released under the **Creative Commons Attribution 4.0 International (CC BY 4.0)** license.

Under this license, users may share, adapt, and use the dataset, including commercially, provided they comply with the license terms and give appropriate attribution.

**Attribution:** Divya Ramnani — Signova Hand Gesture Dataset

[Read the CC BY 4.0 license](https://creativecommons.org/licenses/by/4.0/)

*Note: The dataset license applies only to the dataset and does not automatically determine the license for the project's source code.*

##  Models Used

Three deep learning architectures were trained and compared during experimentation.

| Model | Training Accuracy | Validation Accuracy | Remarks |
|---|---:|---:|---|
| CNN | Approximately 86% | Approximately 85% | Selected for real-time use |
| RNN | Approximately 99.8% | Approximately 90.9% | Explored for sequential learning |
| LSTM | Approximately 99.9% | Approximately 99.9% | Computationally heavier |

###  Final Model Choice: CNN

CNN was selected for the image-based gesture recognition prototype because:

- The dataset consists of hand gesture images.
- CNNs are suitable for extracting spatial image features.
- The model was selected with real-time performance and computational cost in mind.

Reported accuracy values are based on project experiments and may vary with the dataset split and evaluation conditions.

##  Features

- 📷 Real-time hand gesture recognition using a webcam.
- 🔁 Two-way communication workflow.
- 🧠 CNN-based deep learning model.
- 📝 Gesture-to-text conversion.
- 🎞️ Text-to-ISL GIF conversion.
- 💻 No specialized external hardware required.

##  Technology Stack

- Python
- TensorFlow / Keras
- OpenCV
- MediaPipe
- NumPy
- Matplotlib
- Deep Learning (CNN, RNN, LSTM)

##  Limitations

- Currently supports only 12 predefined gesture classes.
- Recognition performance may vary with lighting, background, and hand positioning.
- The current recognition model focuses on static gestures.
- Continuous and dynamic sign language recognition requires further development.
- Recognition accuracy may vary in real-world environments.

##  Future Enhancements

- Expand the dataset with more gesture classes and variations.
- Improve robustness using more diverse training images.
- Add dynamic and continuous sign language recognition.
- Develop a mobile application.
- Explore regional sign language variations.
- Improve accessibility and real-world usability.

##  Research Paper

This project is associated with the following research paper:

[Read the Research Paper](https://drive.google.com/file/d/1XpfLapwE3EMod1H7S3rmuE991q-UMRRr/view?usp=sharing)

##  Contributions

Contributions, suggestions, and improvements are welcome.

If you use the dataset, please follow its license terms and provide appropriate attribution to the original creator.

You can fork this repository, experiment with the project, and submit a pull request with improvements.

##  Final Note

Signova aims to explore how deep learning and computer vision can support more inclusive and accessible communication.

The dataset is shared to encourage other students, developers, and researchers to learn, experiment, and build upon this work.

If this project inspires you, consider giving the repository a ⭐ star!
