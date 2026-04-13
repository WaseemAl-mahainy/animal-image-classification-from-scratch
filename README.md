# Animal Image Classification from Scratch

A solo deep learning project that builds and evaluates a custom convolutional neural network (CNN) for classifying 10 animal categories from the Animals-10 dataset using TensorFlow/Keras.

##  Project Overview

This project focuses on image classification using a CNN built entirely from scratch rather than relying on a pretrained backbone. The goal was to understand the full deep learning pipeline for computer vision, including data preparation, augmentation, model design, hyperparameter tuning, training optimization, and evaluation.

The model was trained to classify images into 10 animal classes:
- butterfly
- cat
- chicken
- cow
- dog
- elephant
- horse
- sheep
- spider
- squirrel

## Dataset

- **Dataset:** Animals-10
- **Task:** Multi-class image classification
- **Train images:** 25,149
- **Test images:** 9,447

## Tech Stack

- Python
- TensorFlow / Keras
- NumPy
- Matplotlib
- scikit-learn
- Jupyter Notebook

## Methodology

The project includes a full image classification workflow:
- dataset preparation and train/test splitting
- image preprocessing and augmentation
- multiple CNN experiments with architectural changes
- hyperparameter tuning across epochs, batch size, dropout, and regularization
- training improvements using checkpointing, early stopping, and dynamic learning-rate reduction
- final model evaluation using class-wise metrics and overall accuracy

## Model Development

Several experiments were conducted to improve performance, including:
- increasing and reducing batch size
- adding more convolutional layers
- changing the number of neurons
- applying dropout and regularization
- increasing training epochs
- using callbacks such as:
  - ModelCheckpoint
  - EarlyStopping
  - ReduceLROnPlateau

## Results

The final evaluated model achieved approximately:

- **Test Accuracy:** 89%
- **Weighted F1-score:** 0.89
- **Macro F1-score:** 0.88

### Example class-wise results
- butterfly: 96.39%
- dog: 91.58%
- horse: 94.21%
- spider: 95.36%
- sheep: 64.52%

These results show strong overall classification performance, with some classes performing better than others depending on visual similarity and dataset complexity.

## Files in This Repository

- `from_scratch_animal_classifier.ipynb` — complete notebook for preprocessing, training, and evaluation
- `sample_outputs/` — optional screenshots or result figures
- `test_images/` — optional small set of demo images
- `requirements.txt` — Python dependencies

## How to Run

1. Clone the repository
2. Install dependencies from `requirements.txt`
3. Open the notebook
4. Download the Animals-10 dataset
5. Update dataset paths if needed
6. Run the notebook cells in order

## Future Improvements

- improve performance on difficult classes such as sheep
- test deeper custom CNN architectures
- compare results with pretrained transfer learning models
- export the best model into a deployment-ready inference pipeline

## Author

**Waseem Al-Mahainy**  
AI / Machine Learning student engineer
