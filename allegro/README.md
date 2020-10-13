# Allegro 

This is complimentary to Moses Guttmann presentation on 10/08/2020 on the MLOps class.



## Class How To

* Find your password at `student_keys` file 
* Your username is your UofC username.
* Log in into https://app.uchicago.hosted.allegro.ai/
    * Accept the EULA
    * Click top right
    * Create New Credentials
* Create a new conda environment with the basic libraries you normally use.
* Run:  
```bash
pip install -U --extra-index-url https://shared:HF6w0RbukY@allegroai.jfrog.io/allegroai/api/pypi/public/simple allegroai
allegroai-init

pip install -U trains-agent
trains-agent init
```



## Getting Started
This is the allegro how-to. You will only be able to see it after logging in.
https://app.uchicago.hosted.allegro.ai/docs/getting_started/getting_started_overview/

## Homework 

1. Install the allegroai package
`pip install --extra-index-url https://uchicago:wBTvRsWpSYE5UG2@allegroai.jfrog.io/allegroai/api/pypi/public/simple allegroai==3.3.1`

2. Fork of the original "YOLO KITTI-2d-object-detection":
`https://github.com/alguchg/KITTI-2d-object-detection`

3. Change "detect.py" script to run over the "Test dataset" and produce visualization of the detections.

4. Register back the detection and create a new version of the test dataset, with the automatic detections as annotations.

5. Apply that on a picture from your cellphone =)

## Questions?

* What is allegro?
* How to install on windows?
* How to install on mac?
* What are the basic functions on your local server?
* What is the Kitti2D dataset?

## Data Pre Processing

* Splitting the train / validation dataset. What are the considerations we want to make our model as good as it can be?

* Publishing <<>> Commiting. It does lock the state of the data and recquire the user to 

## Training 

* Train.. Train.. Train.. 
* PyTorch is awesome right?

## Inference 

* Which data do we use?
* Which metric do we use for assessing quality?

## Automation