# Allegro 

This is complimentary to Moses Guttmann presentation on 10/08/2020 on the MLOps class.

## Class How To

* Find your password at ./student_keys.json (your username is your UofC LDAP username).
* https://app.uchicago.hosted.allegro.ai/
..* Accept the EULA
* Click top right
..* Create New Credentials
* Run the first pip for installing and configuring the Allegro AI SDK (Software Development Kit) & the second for installing and configuring the Execution Agent
```bash
pip install -U --extra-index-url https://shared:HF6w0RbukY@allegroai.jfrog.io/allegroai/api/pypi/public/simple allegroai
allegroai-init

pip install -U trains-agent
trains-agent init
```
Additional installation/setup details and answers to common questions can be found at the link in the below "Getting Started" section.


## Getting Started
This is the allegro how-to. You will only be able to see it after logging in.
https://app.uchicago.hosted.allegro.ai/docs/getting_started/getting_started_overview/

## Homework 

1. Install the allegroai package
`pip install --extra-index-url https://uchicago:wBTvRsWpSYE5UG2@allegroai.jfrog.io/allegroai/api/pypi/public/simple allegroai==3.3.1`

2. Fork of the original "YOLO KITTI-2d-object-detection":
`https://github.com/alguchg/KITTI-2d-object-detection`
2.1. Is the public KITTI dataset on the system already?

3. Change "detect.py" script to run over the "Test dataset" and produce visualization of the detections.
3.1  Is this the only file that we are supposed to have to change?  Because I'm getting errors related to other files--main, parse_model_config.  Is fixing those issues part of the assignment? 
3.2  Do we need to change the weights as well?   

4. Register back the detection and create a new version of the test dataset, with the automatic detections as annotations.

5. Apply that on a picture from your cellphone =)

## Questions?

* What is allegro?
* How to install on windows?
* How to install on mac?
* What are the basic functions on your local server?

## Data Pre Processing

* Splitting the train / validation dataset. What are the considerations we want to make our model as good as it can be?

* Publishing <<>> Commiting. It does lock the state of the data and recquire the user to 

## Training 

* Train.. Train.. Train.. 
* PyTorch is awesome right?
Well, I was trained on tensorflow for ML, so not sold yet.  But if anyone else wants the result of my Google search, here's a comparison:  https://realpython.com/pytorch-vs-tensorflow/

## Inference 

* Which data do we use?
* Which metric do we use for assessing quality?

## Automation
