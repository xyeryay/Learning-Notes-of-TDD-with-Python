## 1. What is FT?
FT can be a sort of specification for your application. It tends to track what you might call a User Story, and follows how the user might work with a particular feature and how the app should respond to them.

Functional Test == Acceptance Test == End-to-End Test. Another term is black box test, because the test doesn’t know anything about the internals of the system under test.

FTs should have a human-readable story that we can follow. We make it explicit using comments that accompany the test code. 

When creating a new FT, we can write the comments first, to capture the key points of the User Story.

The minimum viable app is the simplest thing we can build that is still useful.

## 2. Good comments
The ideal is to strive to make your code so readable, to use such good variable names and function names, and to structure it so well that you no longer need any comments to explain what the code is doing. Just a few here and there to explain why.

We use comments to explain the User Story in our functional tests—by forcing us to make a coherent story out of the test, it makes sure we’re always testing from the point of view of the user

## 3. unittest Module
![image](https://github.com/xyeryay/Learning-Notes-of-TDD-with-Python/blob/main/images/use-unittest-module.PNG)</br>
 (1). It inherits from unittest.TestCas.</br>
 (2). Any method whose name starts with test is a test method, and will be run by the test runner. setUp and tearDown are special methods which get run before and after each test. They’re a bit like a try/except.</br>
 (3). self.fail just fails no matter what, producing the error message given. It is used as a reminder to finish the test.</br>
 (4). It will an expected fail
 
 ## 4. TDD Concepts
**User Story** </br>
A description of how the application will work from the point of view of the user. Used to structure a functional test.

**Expected failure** </br>
When a test fails in the way that we expected it to.
