## 1. Required Software Installations
To finish the project in this book. You need to install:
#### 1.	Python. 
Python 3 is better.
#### 2.	The Firefox web browser
#### 3.	The Git version control system
On Windows, this comes with the Bash command line, which is needed for the book. All the following commands will be executed on "Git Bash".
#### 4.	The virtualenv with Python 3, Django 1.11, and Selenium 3 in it
#### 5.	Geckodriver
This is the driver that will let us remotely control Firefox via Selenium. Download this driver and put it in your folder.

## 2. Setting Up Your Virtualenv
### Install virtualenvwrapper
#### on Windows
pip install virtualenvwrapper
#### on macOS / Linux
#Install virtualenvwrapper at first</br>
pip install --user virtualenvwrapper</br>
#then make Bash load virtualenvwrapper automatically</br>
echo "source virtualenvwrapper.sh" >> ~/.bashrc</br>
source ~/.bashrc</br>
Notes: </br>
(1). On  Windows,  virtualenvwrapper  will  only  work  inside  the  “Git-Bash” shell, not from the normal command line.</br>
(2). virtualenvwrapper keeps all your virtualenvs in one place, and provides convenient tools for activating and deactivating them.</br>
### Let’s create a virtualenv called “superlists”3 that has Python 3 installed:
#### on macOS/Linux:
mkvirtualenv --python=python3.6 superlists
#### on Windows
virtualenv --python=`py -3.6 -c"import sys; print(sys.executable)"` superlists

## 3. Activating and Deactivating the Virtualenv
![image](https://github.com/xyeryay/Learning-Notes-of-TDD-with-Python/blob/main/images/activate-deactivate-virtualenv.png)</br>
**Note that all the following commands should be executed in the activated virtualenv.**</br>

## 4. Install Django and Selenium 
![image](https://github.com/xyeryay/Learning-Notes-of-TDD-with-Python/blob/main/images/install-django-selenium.png)
