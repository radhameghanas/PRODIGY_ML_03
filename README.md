Cat vs Dog Image Classification

This project uses Support Vector Machines (SVM) to classify images of cats and dogs. The dataset consists of images organized into two folders: Cat and Dog. The images are preprocessed, flattened, and used to train an SVM model with a polynomial kernel.

Table of Contents
Installation
Usage
Dataset
Model Training
Model Testing
Results

Clone the repository:
git clone (https://github.com/radhameghanas/PRODIGY_ML_03)
cd your-repo

Create and activate a virtual environment (optional but recommended):
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`

Install the required dependencies:
pip install numpy opencv-python matplotlib scikit-learn

Usage
Prepare your dataset:
Organize your images into two folders: Cat and Dog within a parent folder named Dataset.

Dataset/
├── Cat/
│   ├── cat1.jpg
│   ├── cat2.jpg
│   └── ...
└── Dog/
    ├── dog1.jpg
    ├── dog2.jpg
    └── ...
    
Run the script:
python your_script.py

Dataset
The dataset should be organized into two folders: Cat and Dog. Each folder should contain images of the respective category.

Model Training
The script preprocesses the images by resizing them to 100x100 pixels, converting them to grayscale, and flattening them into a 1D array. It then splits the data into training and testing sets and trains an SVM model with a polynomial kernel.

Model Testing
After training, the model's accuracy is evaluated on the test set. The script also makes a prediction on a sample test image and displays it along with the predicted label.

Results
An example output of the script:
Accuracy: 0.5454545454545454
Prediction is Dog
The test image is displayed using matplotlib.
