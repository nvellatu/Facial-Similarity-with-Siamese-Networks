I worked alongside two classmates to design Siamese networks trained to verify a student's identity. 
## In practice:
- First, take a picture of yourself.
- Take a picture of your ID card
- An image processing function will extract the ID# from the image of the ID card.
- A search will be run on our mock database to find the corresponding stored image for that ID#
- The camera-captured image along with the stored image will be run through our model to produce a "dissimilarity score", which measures how different the people in the two images are.
- Generally, a score <1 means that the student passes the verification and matches the stored image; a score >1 generally means that the student fails the verification and the two images are of different people. 

The model is not 100% accurate due to limited training images (only 370 images of 37 people used for training). Still, we believe we have increased its accuracy by using a pre-trained VGG model as well as augmenting the training data.

For more information look at our report titled "Implementing_Facial_Recognition_Technology_for_Student_ID_Verification.pdf"


## Installing the right version of PyTorch 
This project is updated to be compatible with pytorch 0.4.0



#### This project requires python3.6

