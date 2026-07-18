# Student-Attentiveness-Detection

Student attentiveness plays a vital role in enhancing learning outcomes in both traditional and online classrooms. This project presents a deep learning-based system that automatically predicts students' attentiveness by analyzing their facial expressions. Using facial emotion recognition, the system classifies student engagement into five categories: Focused, Confused, Bored, Sleepy, and Deviated.

The project employs DenseNet121, a powerful convolutional neural network, to accurately recognize facial emotions from classroom images. The predicted emotions are further utilized to evaluate the overall engagement level of students during learning sessions.



**Features**
Automatic facial emotion recognition using deep learning.
Student attentiveness classification into five categories.
Image preprocessing and data augmentation techniques.
DenseNet121-based classification model.
Training and validation pipeline.
Performance evaluation using Accuracy, Precision, Recall, and F1-Score.
Confusion Matrix and ROC-AUC curve visualization.
Overall Engagement Index (OEI) and Random Engagement Index (REI) calculation.
Prediction on unseen images with confidence scores.



 **Technologies Used**
 
Programming Language
Python 3.x
Deep Learning Framework
PyTorch
TorchVision
Computer Vision
OpenCV
PIL (Python Imaging Library)
Data Processing
NumPy
Pandas
Visualization
Matplotlib
Machine Learning
Scikit-learn



 **Dataset**

The model is trained on a classroom facial emotion dataset consisting of 10,736 images categorized into the following classes:

Focused
Confused
Bored
Sleepy
Deviated

The dataset is preprocessed by resizing images to 224 × 224 pixels, followed by normalization and data augmentation to improve the model's generalization capability.




**Workflow**

Collect classroom facial images or video frames.
Detect and crop student faces from the images.
Resize images to 224 × 224 and apply preprocessing techniques.
Perform data augmentation to improve model robustness.
Train the DenseNet121 model using the processed dataset.
Validate the trained model using the validation dataset.
Predict the facial emotion of students from new images.
Classify the attentiveness level into one of the five categories.
Evaluate the model using Accuracy, Precision, Recall, F1-Score, Confusion Matrix, and ROC-AUC Curve.
Calculate the Overall Engagement Index (OEI) and Random Engagement Index (REI) for engagement analysis



**Model Architecture**

The proposed system utilizes DenseNet121, a densely connected convolutional neural network that promotes efficient feature reuse and alleviates the vanishing gradient problem. Its architecture enables effective extraction of facial features, making it well-suited for facial emotion recognition tasks.

Training Configuration
Parameter	Value
Model	DenseNet121
Image Size	224 × 224
Batch Size	32
Epochs	35
Optimizer	Adam
Loss Function	CrossEntropyLoss
Number of Classes	5

**Evaluation Metrics**
Accuracy
Precision
Recall
F1-Score
bounding boxes along with the confidence score 
Confusion Matrix
ROC-AUC Curve
Overall Engagement Index (OEI)
Random Engagement Index (REI)
Inference Time
