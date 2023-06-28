<h1 align="center">Similar Fashion Image Recommendation</h1>

<p align="center">
  <img src="placeholder_image" alt="Project Preview" width="600">
</p>

<p align="center">
  <strong>Enhance product discovery with visually similar fashion images.</strong>
</p>

## Table of Contents
- [Project Overview](#project-overview)
- [Project Architecture](#project-architecture)
- [Technology Stack](#technology-stack)
- [Implemented Features](#implemented-features)

## Project Overview

The Similar Fashion Image Recommendation project is inspired by the similar image recommendation feature in Gmarket. The goal is to overcome the limitations of existing deep learning-based image classification, such as execution time, cost, and disk storage.

### What is Similar Image Recommendation?

Gmarket App introduced the Similar Image Recommendation feature in May 2022. Instead of showing identical product images, this feature displays visually similar images to help users discover products more easily.

![Similar Image Recommendation](placeholder_image)

We aim to experiment with creating a closed-source similar image site to provide users with fast and easy access to visually similar fashion images.

## Project Architecture

<p align="center">
  <img src="placeholder_image" alt="Project Architecture" width="800">
</p>

## Technology Stack

- Front-end: React (Web page UI, interface implementation)
- Front-end: Figma (Web page UI, design prototyping)
- Back-end: Flask (API communication with the server)
- Back-end: Weaviate (Storing image datasets in a vector space using Docker)
- Back-end: TensorFlow (Training image datasets using the TensorFlow CNN model)

## Implemented Features

### I. Front-end

#### 1. Version 1 - Bootstrap-based Menu Bar and Main Window UI
![Version 1](placeholder_image)

#### 2. Version 2 - Improved User Interface with Result Images Display and Modal Window
![Version 2](placeholder_image)

### II. Back-end and API Communication

#### 1. Request Functions
![Request Functions](placeholder_image)

#### 2. Response Function
- Reads the data from the request's body, performs label prediction by passing the image data to the CNN model.
![Response Function](placeholder_image)

#### 3. Vector Database
- Uses Weaviate's vector database to retrieve similar image results based on the input query image and labels.
![Vector Database](placeholder_image)

#### 4. Server Setup
- Started the server following these steps:
  - Launched Docker to run Weaviate.
  - Defined the schema for image information.
  - Converted all images into base64 format and imported them into Weaviate.
![Server Setup](placeholder_image)

- Weaviate running on Docker Desktop.
![Weaviate Running](placeholder_image)

- Directory path where the images were stored as base64 versions.
![Base64 Images Directory](placeholder_image)

- Imported all images into Weaviate. (Performed individually for each of the 6 image categories)
![Importing Images](placeholder_image)

- Running the server. (python flask-app/application.py)

---

