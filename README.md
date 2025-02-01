# Week-2
1. **Import Libraries**: Necessary libraries like OpenCV, TensorFlow, Pandas, Matplotlib, and NumPy are imported.  
2. **Define Paths**: `train_path` and `test_path` are set to the dataset directories.  
3. **Load Data**: Images from the `train` folder are read using OpenCV, converted to RGB, and stored in `x_data`, with labels stored in `y_data`.  
4. **Create DataFrame**: A Pandas DataFrame is created with images and labels.  
5. **Visualize Data**: A pie chart shows the class distribution, and sample images are displayed.  
6. **Build CNN Model**: A `Sequential` model is created with three convolutional layers, ReLU activations, and max pooling.  
7. **Flatten and Dense Layers**: The output is flattened, followed by fully connected layers with dropout for regularization.  
8. **Output Layer**: A dense layer with 2 nodes (for binary classification) and a sigmoid activation is added.  
9. **Compile Model**: The model is compiled with binary cross-entropy loss, Adam optimizer, and accuracy metric.  
10. **Data Augmentation**: `ImageDataGenerator` is used to rescale images.  
11. **Prepare Data Generators**: `flow_from_directory` loads images from directories and resizes them to (224, 224).  
12. **Check Data**: The number of images in training and testing sets is displayed.  
13. **Train Model**: The model is trained for 10 epochs using `train_generator` and validated using `test_generator`.  
14. **Monitor Training**: The training progress is stored in `hist`.  
15. **Optimize for Speed**: Training can be sped up by reducing image size, batch size, or using a GPU.
