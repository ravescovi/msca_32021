# Allegro 

This is complimentary to Moses Guttmann presentation on 10/08/2020 on the MLOps class.

Students should fork & clone this repository by:
1) Navigating to Rafael's msca_32021 repository 
2) Forking it 
    - Note: This creates a new copy of my demo repo under your GitHub user account, including all the code, branches & commits from the original repo
3) Then cloning it to your local system by: 
    1) On GitHub, navigating to the main page of YOUR copy of the repository
    2) Clicking on the green code button
    3) Clone with HTTPS, SSH or GitHub CLI
    4) Openning terminal & changing the current working directory to the location where you want the cloned directory
    5) Typing: git clone & pasting the URL copied earlier
            e.g., git clone [insert your location here]
    6) Pressing Enter
4) Making a new branch
        e.g., git checkout -b [the desired name for your new branch]
5) Create a new remote for the upstream repo
    - Note: "upstream repo" refers to the original repo you created your fork from
    - Do this by the following command: git remote add upstream [link to Rafael's original repository]
6) Making your changes
7) Pushing it to your repository
8) Clicking the Compare & pull request button (this will be present on Rafael's version of the repo)
9) Clicking create pull request to open a new pull request



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
    Note: If you are on a Mac and receive the following error when running detect.py but are confused since you feel you already installed allegroai per the abo ve command, realize that pip comes pre-installed with Python 2.7. Pip3 is the Python3 version of pip. You have to use pip3 for it to be installed on Python3 and avert this error (assuming all over your other install steps were correct, of course):
        File "src/detect.py", line 26, in <module>
        from allegroai import Task, DataView, DatasetVersion
        ModuleNotFoundError: No module named 'allegroai'

2. Fork of the original "YOLO KITTI-2d-object-detection":
`https://github.com/alguchg/KITTI-2d-object-detection`
2.1. Is the public KITTI dataset on the system already?
(remember to clone only the allegro branch to your local directory; you can use the following command: git clone -b allegroai https://github.com/YOURUSERNAMEHERE/KITTI-2d-object-detection.git)
    - Note: to quickly install all of the dependencies in requirements.txt, simply run the command:
        pip install -r requirements.txt

3. Change "detect.py" script to run over the "Test dataset" and produce visualization of the detections.
    - Note: latest version of script leverages a batch_size of 2; during training you will also see at "data size" of 5; in combination, this should produce 10 output images

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

## Inference 

* Which data do we use?
* Which metric do we use for assessing quality?

## Automation