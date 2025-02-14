# Text-Identifier
This project implements a deep learning model to classify handwritten characters. The dataset is segmented for efficient training, and the model is built using TensorFlow and Keras. The final output includes both classification results and a Pygame-based user interface for real-time input and recognition.

# Process
Trains model using an online dataset of 300,000+ individually labeled characters  
Data is split into **80% training** and **20% testing** to evaluate accuracy.  
The model is trained in multiple epochs, adjusting weights to minimize classification errors.  

# Model Specifics
A Multi-Layer Perceptron (MLP) is used with three dense layers:  
- Input Layer: 784 neurons (28x28 flattened image input)  
- Hidden Layers: 128 and 64 neurons (ReLU activation)  
- Output Layer: 26 neurons (softmax activation for classification)  
The model is trained using categorical cross-entropy loss and Adam optimizer.  

# Code and Libraries
TensorFlow / Keras: Deep learning model implementation.  
Pandas / NumPy: Data loading and preprocessing.  
Scikit-learn: Train-test splitting.  
Pygame: User interface for drawing and recognition.  

# Results
The model achieves ~95% accuracy on test data.  
Real-time character recognition is supported through Pygame, allowing users to draw and classify handwritten input interactively.
