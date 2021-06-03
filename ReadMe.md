# Instruction on how to set-up environment for expero 360-healthcare project in windows

## Author
James Li, Lynn Niu

## Git
If you don't have git installed, download and install git from the official website 
https://git-scm.com/downloads

## Editor
We are using Pycharm

## Step1 - Accept invitation
Accept invitation for the github repos. 

## Step 2 - Get from VCS
## 2.1 
Open a repo
## 2.2 
Click on the green button “code” and copy the https url
## 2.3 
In cmd, cd to the directory where you would like to check out the repos
## 2.4 
	git clone <url>
## 2.5 
cd into the repo’s directory
## 2.6 
	git checkout dev/public

Repeat these steps for all repositories.

## Step 3 - More files
Place docker-compose.yml, start.py and version.txt (“v1.0.19-dhei”) at root (same level as 4 repos)

## Step 4 - Set-up anaconda virtual environment 
following the instructions on (using pycharm) https://www.jetbrains.com/help/pycharm/conda-support-creating-conda-virtual-environment.html#8e4c49f7

## Step 5 - Build and Run
## 5.1 Navigate to your virtual environment
## 5.2
	pip install click
## 5.3
If you don' t have docker desktop already, download from https://docs.docker.com/get-docker. 
Make sure Docker desktop is running in the background 
(or conda install -c conda-forge docker-compose if you have conda added in you system path)
## 5.4 
place credentials.json in 360-healthcare-backend/bigquery (if you see some other folders with the same name, 
double check your branch!)
## 5.5
	python start.py build
## 5.6 
	python start.py up

## Step 6
Go to http://localhost:8080/ and see the app


