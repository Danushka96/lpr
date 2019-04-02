# LPR

License Plate Recognition System with Machine Learning in Python

## Dependencies

1. [Numpy](http://docs.scipy.org/doc/numpy-1.10.0) :Numpy is a python package that helps in handling n-dimensional arrays and matrices
1. [Scipy](http://scipy.org/) :Scipy for scientific python
1. [Scikit-image](http://scikit-image.org/): Scikit-image is a package for image processing
1. [Scikit-learn](http://scikit-learn.org/) Scikit-learn is for all machine learning operations
1. [Matplotlib](http://matplotlib.org/) Matplotlib is a 2D plotting library for python

## How to Install

1. Clone this Repository
2. Go to the extracted folder
3. Install all the necessary dependencies by using
<b>`pip install -r requirements.txt`</b>

## How to Run

#### For a better undestaing what's going on with these scripts follow this order

1. `python3 localization.py` With this you can change the images in test folder and changing the line 
`car_image = imread("test\car1.jpg", as_grey=True)`
with your own name. Functionality of this scipt is greyscale the picture given

![](https://i.imgur.com/reM5iLg.png)




2. `python3 cca2.py` This script imports the previous one for getting the greyscale image. So this will open another window with previous result which can be commented if you don't need that

![](https://i.imgur.com/0QsXUx8.png)


3. `python3 segmentation.py` Number plate detection is made manually here. 
`license_plate = np.invert(cca2.plate_like_objects[2])`
However if the license plate is not detected you will have to change this index 2 to the licenseplate box number

![](https://i.imgur.com/wq435Iv.png)


4. `python3 machine_train.py` Training process with data in the train folder is done with this script.

![](https://i.imgur.com/We6FyjU.png)


5. `python3 prediction.py` Given image's (car1.jpg) License plate number will be visible in the terminal output in here

![](https://i.imgur.com/1Lk4muI.png)


## References

[SQUARE](https://blog.devcenter.co/developing-a-license-plate-recognition-system-with-machine-learning-in-python-787833569ccd) <br/>
[femioladeji](https://github.com/femioladeji/License-Plate-Recognition-Nigerian-vehicles)


## Any kind of contribution for this project is welcome.. :D

#happyCoding


