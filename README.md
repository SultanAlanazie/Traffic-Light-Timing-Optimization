# Traffic-Light-Timing-Optimization

## Project Introduction

This project aims to optimize traffic light timing by detecting vehicles and analyzing their distribution at intersections. Using a YOLO-based object detection model combined with KMeans clustering, the system identifies groups of vehicles near traffic lights to estimate congestion and support smarter traffic control strategies.

## Dataset & Input

- Input images of intersections with vehicles.

- Vehicle detection performed using a pre-trained YOLO model.

- Cluster analysis applied to detected vehicle positions for congestion estimation.

## Structure

- **YOLO Detection**: Identifies vehicles in uploaded images.

- **KMeans Clustering**: Groups detected vehicles into clusters to approximate waiting lines near traffic lights.

- **Visualization**: Bounding boxes and cluster colors overlaid on the image, with vehicle counts per cluster displayed.

## Objective

The primary goal is to provide a data-driven method for optimizing traffic light cycles by estimating vehicle density and distribution, reducing congestion and improving traffic flow efficiency.

## Methodology

1- **Object Detection**

- YOLO model detects vehicles in the uploaded image.

- Extracts bounding boxes, centroids, and confidence scores.

2- **Clustering**

- Vehicle centroids are grouped using KMeans clustering.

- Each cluster represents a traffic lane or group of vehicles waiting at the light.

3- **Visualization & Analysis**

- Bounding boxes drawn with cluster-specific colors.

- Vehicle counts per cluster displayed directly on the image.

## Deployment

- Implemented as a **Streamlit app** for user-friendly interaction.

- Users can upload an image, select the number of clusters, and visualize vehicle distribution in real-time.
