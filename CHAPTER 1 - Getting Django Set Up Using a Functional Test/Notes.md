## 1. Testing Goat
#### 1. The Testing Goat is the unofficial mascot of TDD in the Python testing community.
#### 2. When  you’re  doing  TDD,  you  always  have  the Testing Goat inside you—single-minded as goats are—bleating “Test first, test first!”
#### 3. In TDD the first step is always the same: write a test. Another thing about goats is that they take one step at a time. 

## 2. First Functional Test(FT)
In your folder, create a  new  Python  file  called  functional_tests.py, and enter the following code.

from selenium import webdriver</br>
browser = webdriver.Firefox()</br>
browser.get('http://localhost:8000')</br>
assert 'Django' in browser.title</br>

Run it:</br>
![image](https://github.com/xyeryay/Learning-Notes-of-TDD-with-Python/blob/main/images/run-first_ft.png)</br>
You should see a browser window pop up and try to open localhost:8000, and show the “Unable to connect” error page. 

## 3. Getting Django Up and Running
Django provides a little command-line tool to create a project.
![image](https://github.com/xyeryay/Learning-Notes-of-TDD-with-Python/blob/main/images/create-a-django-project.png)</br>

That will create a folder called superlists, and a set of files and subfolders inside it:</br>
![image](https://github.com/xyeryay/Learning-Notes-of-TDD-with-Python/blob/main/images/files-in-superlists-project.PNG)</br>
There’s a folder called superlists inside a folder called superlists. The important thing to know is that the superlists/superlists folder is for stuff that applies to the whole project. </br>
manage.py. is used to run a development server.
![image](https://github.com/xyeryay/Learning-Notes-of-TDD-with-Python/blob/main/images/run-development-server.png)</br>

That’s Django’s development server now up and running on our machine. Leave it there and open another command shell. In that, we can try running our test again(from the folder we started in):</br>
$ python functional_tests.py</br>

A new terminal window is opened without AssertionError.</br>
![image](https://github.com/xyeryay/Learning-Notes-of-TDD-with-Python/blob/main/images/first-django-powered-page.PNG)

### 4. Using Git as our VCS
(1). Move functional_tests.py into the superlists folder</br>
(2). Do the **git init** to start the repository. The top-level superlists folder will be our working directory</br>
(3). Take a look and see what files we want to commit</br>
(4). Add some files to a special file called .gitignore which tells Git what to ignore</br>
(5). Add the rest of the contents of the current folder</br>
(6). Remove .pyc files from Git and add them to .gitignore too</br>
(7). Do our first commit</br>
(8). When you type git commit, it will pop up an editor window for you t  write your commit message in</br>
![image](https://github.com/xyeryay/Learning-Notes-of-TDD-with-Python/blob/main/images/start-a-git-repo.png)
