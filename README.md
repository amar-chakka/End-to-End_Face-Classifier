> # Face Identification 

![enter image description here](https://github.com/amar-chakka/End-to-End_Face-Classifier/blob/d2e891ececb28f320c5bd6a50db67e4456de25ee/face_recog.jpg?raw=true)


**The objective of this project is to:**

**The client for this project is the Administration Department at AutoBox having over a thousand employees. They want to supplement their current process with  a more proactive approach**

They want to maintain a central database of all of their employees. And, extra emphasis is on increasing security and ease of operation. The idea is to create a web-based app for Facial Recognition in order to have rightful entry to the office premises and restrict any trespassers. Once the employees are identified on a daily basis, they can have a simple entry and exit procedure without any manual intervention. They want to deal with their existing employee’s database and those coming in as a new recruit.

**Current Practice:**

The existing employees or the ones joining the Company gets a card having a QR(RFID) code with unique identification for entry and exit.

The current practice suffers from the following problems:

This approach is too haphazard. The quality of insight gained is misaligned due to misleading data. The second problem is these insights can't be aggregated to frame certain policies on this. The third problem is the security breach of the Company, which can hamper the situation very badly.

The Admin Department has hired you as an AI Engineer. They want to supplement their security protocols with a more proactive approach.

**Problem Specifics**
Detecting and Identifying the face is an important and key challenge in Face recognition. Analysis in this area is plagued by issues related to different image sizes, brightness and other visual dimensions of the images. 

**Deliverable:**  Predict whether the person will be allowed entry or exit into the company premises.

Deep Learning task: Build a Face Recognition model using FaceNet

Target: Predict the name of the person in the image.

**Win condition:**  The model should be able to recognize the person present in the images, and if the model hasn’t seen a person before, it should output a message suggesting that this person is not found in the database and entry is restricted, and label it as Unidentified.


**Observations on dataset:**

-   No. of Celebrities : 18
-   Data sets :  2 [train & validation] 
-   Categorical / Labels: 18
-   No. of Images: 438    

We used ImageDataGenerator with several arguments like rotation_range, horizontal_flip, featurewise_center to generate different images for effective training of the model.

We resized the images to (160,160) such that it fits the need of the "facenet" model specifications.

Used mtcnn package for face extraction from the images.
Loaded images and extract faces for all images in a directory.
Loaded a dataset that contains one subdir for each class that in turn contains images
Got the face embedding using facenet_keras.h5
Trained the model with the embeddings
Finally, developed a classifier model to Identify the name from the listed labels.

Here is a snapshot of the result using the classifier model:

![enter image description here](https://github.com/amar-chakka/End-to-End_Face-Classifier/blob/c3621dc2eba7211c25c69f212c81eb6ba334bbbb/result.JPG?raw=true)







To check out my notebook, please click [here](https://github.com/amar-chakka/End-to-End_Face-Classifier/blob/c3621dc2eba7211c25c69f212c81eb6ba334bbbb/1002_GCDAI_Capstone_Project.ipynb).
