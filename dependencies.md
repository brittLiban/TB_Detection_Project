# Project Dependencies

This document outlines the main dependencies used in the TB Detection Project and provides a brief description of each.

## 1. TensorFlow

- **Version**: 2.x (current version at the time of installation)
- **Purpose**: TensorFlow is an open-source machine learning library developed by Google. We are using TensorFlow to build and train a Convolutional Neural Network (CNN) that can analyze chest X-ray images to detect signs of tuberculosis.
- **Key Features**:
  - Provides tools for building deep learning models.
  - Supports various machine learning algorithms.
  - Includes Keras, a high-level neural networks API that makes it easier to create, train, and evaluate models.

## 2. Flask

- **Version**: 3.x (current version at the time of installation)
- **Purpose**: Flask is a lightweight web framework for Python that helps us build web applications. In this project, we use Flask to create a backend server that accepts X-ray images, processes them using our model, and returns predictions.
- **Key Features**:
  - Simple and flexible, with minimal setup required.
  - Allows for easy routing and handling of HTTP requests.
  - Integrates well with machine learning models for building APIs.

## 3. Flask-CORS

- **Version**: 5.x (current version at the time of installation)
- **Purpose**: Flask-CORS is an extension for handling Cross-Origin Resource Sharing (CORS) in Flask. CORS is a security feature that allows or restricts resources on a web page to be requested from another domain. In our project, Flask-CORS enables our Flask backend to handle requests from a frontend hosted on a different domain.
- **Key Features**:
  - Allows us to enable CORS for specific routes or the entire application.
  - Useful for integrating frontend and backend hosted separately.

## 4. OpenCV (opencv-python-headless)

- **Version**: 4.x (current version at the time of installation)
- **Purpose**: OpenCV is a computer vision library that provides tools for image processing. We use OpenCV to preprocess X-ray images before feeding them to the CNN model.
- **Key Features**:
  - Functions for resizing, transforming, and manipulating images.
  - Optimized for speed and efficiency in image processing tasks.
  - `opencv-python-headless` is a lightweight version of OpenCV without GUI functionality, which is ideal for server environments.

## 5. Pillow

- **Version**: 8.x or higher (current version at the time of installation)
- **Purpose**: Pillow is a Python Imaging Library (PIL) that simplifies image processing tasks. We use it as an alternative to OpenCV for loading and saving images, as well as performing basic manipulations.
- **Key Features**:
  - Supports a wide range of image formats (JPEG, PNG, BMP, etc.).
  - Provides simple tools for resizing, rotating, and converting images.
  - Compatible with TensorFlow and other machine learning libraries.

---

Each of these libraries plays an essential role in our TB detection project, helping us handle everything from image processing to model building and deploying a backend server.
