# Shot_Type_Classification

There are two models available, one _PyTorch implementation_ with 0.90 accuracy trained over 50 epochs, and one _Tensorflow implementation_ with 0.89 accuracy trainned over 12 epochs. The accuracies are based on the testset which were separated from the training set.
Please don't use it for the commersial purposes as the dataset doesn't allow you to do that.


**Model Input/Output**

The trained models are in models folder. And you can test it using `PyTorch_Model_Classifier.ipynb` for PyTorch implementation and `TF_Model_Classifier.ipynb` for TensorFlow implementation.
Both models get an image (or a frame of video) as an input and output the type of shots in one of these 5 categories:

| Class                        | Description                                   |
|------------------------------|-----------------------------------------------|
| Long shot (LS)               | A long distance.                              |
| Full shot (FS)               | Human body in full.                           | 
| Medium shot (MS)             | Knees or waist up.                            |
| Close-up shot (CS)           | A relatively small object, e.g., face, hand.  |
| Extreme close-up shot (ECS)  | Even a smaller parts of object, e.g., eyes    |


Below are some examples of each classes

<div align="center">
  <table border="0" bgcolor="#000000">
      <tr>
        <td valign="top" align="center"><img src="/examples/1.jpg" width="50%"></img> <br />Close-up shot (CS) Example</td>
        <td valign="top" align="center"> <img src="/examples/2.jpg" width="50%"></img> <br />Extreme close-up shot (ECS) Example </td>
        <td valign="top" align="center"> <img src="/examples/3.jpg" width="50%"></img> <br />Full shot (FS) Example </td>
      </tr>
    </table>
    
  <table border="0" bgcolor="#000000">
      <tr>
        <td valign="top" align="center"><img src="/examples/4.jpg" width="50%"></img><br /> Long shot (LS) Example</td>
        <td valign="top" align="center"><img src="/examples/5.jpg" width="50%"></img><br /> Medium shot (MS) Example </td>
      </tr>
    </table>
</div>




**Requirments PyTorch Implementation**

`PyTorch 
Pillow
numpy
torchvision`

**Requirments TensorFlow Implementation**

`tensorflow
OpenCV
numpy
`


**Dataset**

Both models are traned over MovieShots dataset https://paperswithcode.com/dataset/movieshots 
https://arxiv.org/abs/2008.03548


**Model Training**

The codes for training the models are available under training folder.
Steps for training the models again:
1- Download the dataset
2- Follow the steps in `DataSet_CleanUp.ipynb`
3- Train the model by using either PyTorch or Tensorflow implementation file

The pytorch implementation is based on the MRI tumor detection in https://www.kaggle.com/code/oknashar/brain-tumor-detection-using-pytorch?scriptVersionId=90753009&cellId=15
And Tensorflow implementation is based on the MRI tumor detection in https://www.kaggle.com/code/jaykumar1607/brain-tumor-mri-classification-tensorflow-cnn

