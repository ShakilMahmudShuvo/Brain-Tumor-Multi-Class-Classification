# Brain-Tumor-Multi-Class-Classification


Tools : 
- TensorFlow (version 2.11.0)
- NumPy (version 1.24.2)
- Matplotlib (version 3.5.3) 
- TensorBoard (version 2.11.0)
- Keras

Steps: 
  - Dataset Collection
  - Dataset Preprocessing
    - Cropping Brain Contour using various operations such as erotion and dilation
    - Applying bilateralFilter to reuce the noises presented in the edges
    - Resizing  
    - Applying Pseudo-color processing
    - Creating ImageGenerators
    - Model Building : Transfer Learning with ResNet50 Architecture
    - Model Training
    - Performance Evaluation
 
 # Why ResNet50 ? 
 Mainly because of 2 reasons:
 - **Residual connections**: ResNet50 introduces residual connections, which help to prevent the vanishing gradient problem that can occur in very deep networks. This allows for more accurate training and better performance.
 - **Deep**: ResNet50 is a very deep neural network, with 50 layers, allowing it to capture a more complex representation of the input data.
 
 Here is a sample architecture of ResNet50 which was collected from HuggingFace:
![My Image](resnet_architecture.png)

 
 # Dataset Description:
  
  
  Dataset Link: https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset?datasetId=1608934&sortBy=dateRun&tab=profile
  
  
  This dataset contains 7023 images of human brain MRI images which are classified into 4 classes: **glioma - meningioma - no tumor and pituitary.**
