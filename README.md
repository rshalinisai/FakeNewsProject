# Fake News Detection - Multi-Dataset Processing and Feature Engineering

This project handles data processing and feature engineering for detecting fake news using three major datasets: **Fakeddit**, **Weibo**, and **FakeNewsNet**. The goal is to combine text and image data to create a robust feature set for machine learning models.

## Datasets
- **Fakeddit**: A dataset sourced from Reddit, consisting of both rumor and non-rumor posts. Each post contains metadata, text, and images.
- **Weibo**: A collection of tweets from the Weibo platform, labeled as rumors or non-rumors. Each tweet contains metadata, text, and associated images.
- **FakeNewsNet**: A dataset containing news articles with labels indicating whether they are fake or real, along with relevant metadata and images.

## Folder Structure
- `data/`: This folder contains the raw data for the three datasets.
    - `fakenewsnet/`: Processed FakeNewsNet dataset.
    - `weibo/`: Processed Weibo dataset.
    - `fakeddit/`: Processed Fakeddit dataset.
    - `image_dump/`: A folder where all the images from different sources are stored.
- `scripts/`: Python scripts for processing the datasets, performing feature engineering, and saving the processed data.
    - `process_fakeddit.py`: Script to process Fakeddit dataset and scrape Reddit URLs.
    - `process_weibo.py`: Script to process Weibo dataset and scrape article URLs.
    - `process_fakenewsnet.py`: Script to process the FakeNewsNet dataset.
    - `feature_engineering.py`: Code for feature engineering (text and image features).
- `requirements.txt`: Python dependencies needed for the project.
- `.gitignore`: A list of files/folders that should not be committed to the repository (e.g., `.pyc` files, temporary files, etc.).