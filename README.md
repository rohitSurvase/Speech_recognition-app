# Speech_recognition-app
Makes use of speech recognition plugin to recognise the speech through microphone.

# Overview
These are the services for the learning language app written in python.Initially used speech recognition api.
# Steps for virtual environment creation and install Python

# Create Virtual Environment
Let’s start by creating a virtual environment -
cd ~
sudo apt-get install python-virtualenv 
sudo apt-get install python-pip

# Check virtual environment
To check if virtualenv is correctly installed, type -
virtualenv --version

It's time to create to virtual environment flask-env, where we will install flask.

virtualenv flask-env

# Activate Environment
Now let’s activate it using the command below -

source flask-env/bin/activate

# Deactivate Environment
To deactivate the virtual environment, type the below line in the command prompt -

deactivate

# Check Python version
Check for the python version 
python --version

If the python version is 2.0 or lower than 3.0 then install the latest version with following steps.

# Install Latest Python 3.7.3
Run the following steps to download, install and compile the latest version:

# Prerequisites
Use the following command to install prerequisites for Python before installing it:
sudo apt-get install build-essential checkinstall

sudo apt-get install libreadline-gplv2-dev libncursesw5-dev libssl-dev \
    libsqlite3-dev tk-dev libgdbm-dev libc6-dev libbz2-dev

# Download Python 
cd /usr/src
sudo wget https://www.python.org/ftp/python/3.7.3/Python-3.7.3.tgz

# Extract Package
Now extract the downloaded package.

sudo tar xzf Python-3.7.3.tgz

# Compile Python Source
Use below set of commands to compile Python source code on your system using altinstall.

cd Python-3.7.3
sudo ./configure --enable-optimizations
sudo make altinstall

Note : If '_ctypes' module is not found then install libffi-dev by the command:

sudo apt-get install libffi-dev

and again run the altinstall or re install the python with the same steps above.

Tip: make altinstall is used to prevent replacing the default python binary file /usr/bin/python.

# Check Python Version 
Check python version by following commands:

python --version or python3.7 -V

If the version shows Python-3.7.3 which is the latest when documented we are good to go further.

# Installation of Packages which are required to run the services file

#Installation of Flask
sudo pip install Flask

# Installation of speech recognition
sudo pip install SpeechRecognition

#Installation of python pyaudio
First install portaudio
sudo apt-get install libasound-dev

Download the portaudio archive from: http://portaudio.com/download.html

cd /usr/src
sudo wget http://portaudio.com/archives/pa_stable_v190600_20161030.tgz

Unzip the archive:

sudo tar -zxvf pa_stable_v190600_20161030.tgz

Enter the directory, then run: 

./configure && make

Then Install: 

sudo make install

And finally install :

sudo pip install pyaudio

Note: In some cases if not working use below command:

sudo apt-get install python-pyaudio python3-pyaudio

# Import requests Package
sudo pip install requests

