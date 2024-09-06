# Demo-Image-Classifier
Demo of Image-Classifier for Lightbulbs

## Overview
This project is a simple web-based demo that uses a Teachable Machine model to classify images of lightbulbs. The model is loaded in the browser using TensorFlow.js, and users can upload an image (in .png or .jpeg format), which will be analyzed by the model. The predicted class and its probability will be displayed on the screen.

## Features
Teachable Machine Model: The model is trained to classify lightbulb images.
Image Upload: Users can upload an image file for classification.
Real-Time Predictions: Once an image is uploaded, predictions are made instantly, and the results are displayed with their respective probabilities.

## How to Run Locally
### Clone the repository:
```bash
git clone https://github.com/JJblacknight/lightbulb-classifier-demo.git
cd lightbulb-classifier-demo
```

### Open the project in your browser
Open the index.html file in any modern web browser (Chrome, Firefox, Edge, etc.).
You can drag the index.html file directly into the browser or use a local development server such as Live Server in VS Code.

### Upload an image
Once the project is open in the browser, click on the file input button to upload an image in .png or .jpeg format.
After uploading, the model will predict the image and display the class label along with its confidence percentage.

## Dependencies
The project relies on the following external libraries:
+ TensorFlow.js for running the machine learning model in the browser.
+ Teachable Machine Image Library to load and run the image model.
Both of these are included via CDNs:
```bash
<script src="https://cdn.jsdelivr.net/npm/@tensorflow/tfjs@latest/dist/tf.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/@teachablemachine/image@latest/dist/teachablemachine-image.min.js"></script>
```

## Model Information
This demo uses a model exported from Google's Teachable Machine platform. The model is trained specifically to classify lightbulb images, but it can be easily modified to work with other types of image data by changing the model URL.

The model is hosted at:
```ruby
https://teachablemachine.withgoogle.com/models/3F9ShbB8-/
```

## Project Structure
```graphql
lightbulb-classifier-demo/
│
├── index.html       # Main HTML file that contains the interface and script
├── README.md        # Documentation of the project
└── assets/          # (Optional) Directory for any static assets like images
```

## Credits
+ Teachable Machine by Google for making model training and export simple.
+ TensorFlow.js for allowing machine learning models to run directly in the browser.
