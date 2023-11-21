# Image Classification

My ultimate goal is to develop a user-friendly website that enables users to effortlessly drag and drop an image of a sports person. The website will then promptly identify the specific sport associated with the individual in the image. I am focused on classifying images into five distinct categories, featuring my favorite sports celebrities.

To ensure a diverse dataset, I will utilize images sourced from Google, showcasing various sports personalities. This project will guide you through different methods of extracting images from Google. Subsequently, I will delve into feature engineering, employing the renowned image processing library, OpenCV. This exploration will include transformative techniques crucial for training Support Vector Machine (SVM) classifiers and logistic regression classifiers.

While contemporary trends lean towards neural networks for classification tasks, my aim is to illustrate the effectiveness of simpler approaches such as SVM. In this project, I won't delve into deep learning. However, I am considering incorporating neural network-based projects in the future.

In terms of project architecture, we will follow a systematic approach. The initial steps involve building a model, tuning hyperparameters, exporting the model to a file, and subsequently deploying a Python server. The website will interact with this server to provide real-time predictions.

<hr>

Phase 1 : Data Collection

There are four different methods for collecting data from Google:
1. Manual Download: Manually download images from Google Images.
2. Python Web Scraping: Utilize Python and web scraping to automate the downloading of images from Google. Detailed instructions in this article: [Web Scraping for Image Downloading](https://medium.com/geekculture/scrape-google-images-with-python-f9a20cda1355)
3. Chrome Extension (Fatkun): Use a Chrome extension called Fatkun.
4. Purchase from Third-Party Vendors: Purchase images from a third-party vendor selling image databases. In some cases, companies in sports or news domains may have internal databases of these images.

For simplicity purpose, we will be using Chrome Extension (Fatkun).
