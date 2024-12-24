# pca-image-compression

This repository implements image compression using Principal Component Analysis (PCA) from scratch (without using built-in PCA functions like `sklearn.decomposition.PCA`). It covers grayscale image compression, compression of a group of images using eigenfaces, and compression of color images.

## Overview

This project demonstrates how PCA can be used for image compression by reducing the dimensionality of image data. By finding the principal components (eigenvectors with the highest eigenvalues) of the image data, we can represent the image using a smaller set of vectors, achieving compression. The reconstruction process uses these principal components to approximate the original image.

## Task Breakdown

This project is divided into three parts, each implemented in a separate Jupyter Notebook:

*   **`pca.ipynb` (Core PCA for Grayscale Images):** This notebook implements the fundamental PCA algorithm for compressing grayscale images. It includes:
    *   Loading and flattening a grayscale image.
    *   Implementing PCA from scratch: calculating the covariance matrix, eigenvalues, and eigenvectors.
    *   Selecting principal components for dimensionality reduction.
    *   Compressing and reconstructing the image.
    *   Visualizing the original and reconstructed images.
*   **`pca_bonus1.ipynb` (Eigenfaces for Group Image Compression):** This notebook extends the core PCA implementation to compress a set of face images using eigenfaces. It includes:
    *   Loading the Olivetti faces dataset (or any group of similar images).
    *   Calculating eigenfaces (principal components of the face dataset).
    *   Compressing and reconstructing individual face images using the eigenfaces.
    ![image](https://github.com/user-attachments/assets/4ef2503b-76b1-45bc-b0cf-ae4648c2dead)
   
    *   Visualizing the top eigenfaces.
*   **`pca_bonus2.ipynb` (PCA for Color Image Compression):** This notebook adapts the PCA implementation to compress color images by applying PCA to each color channel (R, G, B) separately. It includes:
    *   Loading and splitting a color image into its R, G, and B channels.
    *   Applying PCA to each channel independently.
    *   Compressing and reconstructing each channel.
    *   Merging the reconstructed channels back into a color image.
    *   Visualizing the original and reconstructed color images.

## Dataset

Place your input images in the `data/` directory.

*   `pca.ipynb`: Requires a grayscale image (e.g., a `.png` or `.jpg` file).
*   `pca_bonus1.ipynb`: Uses the Olivetti faces dataset, which is downloaded using `sklearn.datasets.fetch_olivetti_faces()`. You can adapt this to use your own dataset of similar images (e.g., faces, objects).
*   `pca_bonus2.ipynb`: Requires a color image (e.g., a `.png` or `.jpg` file).


## Team Members

*   Zainab Tarek
*   Abdelfattah Mohamed

