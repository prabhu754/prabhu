We have used python(in form of **jupyter notebooks**) for this project.
The notebooks in the base directory are the *main* ones, namely:

- **Data_Exploration.ipynb**: Basic data cleaning and preprocessing on the dataset taken from [MPII dataset](http://human-pose.mpi-inf.mpg.de/) Generates 2 kinds of *csv* for each each class (*Bicycling* and *Walking*). The First feature space contains the distances between each significiant landmarks, the other contains the distances of each of the limbs. A approach of including angles would between each joint will work better on paper, but in practicals it fails as the *viewing angles matter a lot*. If we could get 3D co-ordinate space that would have been way better for the same approch, but I dont think conversion of 2D to 3D image work too well in practice on random Internet Images(small sized images). So accuracy wont be more for the given dataset, but the preprocessing is at best.
- **models.py**: a collections of models are trained on the given training set.
- **testProcessor.ipynb**: takes some test images from `Final Data\img data` and annotates them using `Final Data\posenet_mobilenet_v1_100_257x257_multi_kpt_stripped.tflite` taken from [Pose estimation model Google](https://www.tensorflow.org/lite/models/pose_estimation/overview) and the processed images are saved in `testData` (*Please have a look at them*), it also generates the test data for the same images.

# How to run
### To view the outputs, results and inference, run models.ipynb.


