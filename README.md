# Shot_Type_Classification

There are two models available, one _PyTorch implementation_ with 0.90 accuracy trained over 50 epochs, and one _Tensorflow implementation_ with 0.89 accuracy trainned over 12 epochs. The accuracies are based on the testset which were separated from the training set.


**Model Input/Output**

Models get an image or a frame of video as an input and classify it as one of the following classes:

| Class                        | Description                                   |
|------------------------------|-----------------------------------------------|
| Long shot (LS)               | A long distance.                              |
| Full shot (FS)               | Human body in full.                           | 
| Medium shot (MS)             | Knees or waist up.                            |
| Close-up shot (CS)           | A relatively small object, e.g., face, hand.  |
| Extreme close-up shot (ECS)  | Even a smaller parts of object, e.g., eyes    |

****                       ****

<div align="center">
  <table>
      <tr>
        <td><img src="/examples/1.jpg" width="50%"></img> <br />Close-up shot (CS) Example</td>
        <td> <img src="/examples/2.jpg" width="50%"></img> <br />Extreme close-up shot (ECS) Example </td>
        <td> <img src="/examples/3.jpg" width="50%"></img> <br />Full shot (FS) Example </td>
      </tr>
    </table>
    
  <table>
      <tr>
        <td><img src="/examples/4.jpg" width="50%"></img><br /> Long shot (LS) Example</td>
        <td><img src="/examples/5.jpg" width="50%"></img><br /> Medium shot (MS) Example </td>
        <td> </td>
      </tr>
    </table>
</div>



**Dataset**

Both models are traned over MovieShots dataset https://paperswithcode.com/dataset/movieshots

Classfies each image or videoframe to five categories: 1) long shot (LS) is taken from a long distance, sometimes as far as a quarter of a mile away; 2) full shot (FS) barely includes the human body in full; 3) medium shot (MS) contains a figure from the knees or waist up; 4) close-up shot (CS) concentrates on a relatively small object, showing the face of the hand of a person; (5) extreme close-up shot (ECS) shows even smaller parts such as the image of an eye or a mouth.
