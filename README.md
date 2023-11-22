# Image Classification

Our ultimate goal is to develop a user-friendly website that enables users to effortlessly drag and drop an image of a sports person. The website will then promptly identify the specific sport associated with the individual in the image. We will be focused on classifying images into five distinct categories, featuring famous sports celebrities.

To ensure a diverse dataset, we will utilize images sourced from Google, showcasing various sports personalities. Subsequently, we will delve into feature engineering, employing the renowned image processing library, OpenCV. This exploration will include transformative techniques crucial for training Support Vector Machine (SVM) classifiers and logistic regression classifiers.

While contemporary trends lean towards neural networks for classification tasks, our aim is to illustrate the effectiveness of simpler approaches such as SVM. In this project, we won't delve into deep learning. However, we will be incorporating neural network-based projects in the future.

In terms of project architecture, we will follow a systematic approach. The initial steps involve building a model, tuning hyperparameters, exporting the model to a file, and subsequently deploying a Python server. The website will interact with this server to provide real-time predictions.

<hr>

Phase 1 : Data Collection

There are four different methods for collecting data from Google:
1. Manual Download: Manually download images from Google Images.
2. Python Web Scraping: Utilize Python and web scraping to automate the downloading of images from Google. Detailed instructions in this article: [Web Scraping for Image Downloading](https://medium.com/geekculture/scrape-google-images-with-python-f9a20cda1355)
3. Chrome Extension (Fatkun): Use a Chrome extension called Fatkun.
4. Purchase from Third-Party Vendors: Purchase images from a third-party vendor selling image databases. In some cases, companies in sports or news domains may have internal databases of these images.

For simplicity purpose, we will be using Chrome Extension (Fatkun).

<hr>

Phase 2 : Data Cleaning

In the data cleaning process for our project, we prioritize image refinement due to potential issues during the download. Emphasizing the significance of detecting persons in images, our approach involves using facial features like height, hands, and legs. However, the primary focus is on facial recognition. To ensure clarity, we employ OpenCV, a renowned Python image processing library, utilizing the Haar Cascade technique for precise detection of faces and eyes. Images with a clear face and two eyes are retained, while others are discarded to enhance the accuracy of our face detection process.
