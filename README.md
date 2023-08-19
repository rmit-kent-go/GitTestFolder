# Social Media Analyzer

## Demo Video: https://rmiteduau-my.sharepoint.com/:v:/r/personal/s3955624_student_rmit_edu_au/Documents/Recording-20230819_164953.webm?csf=1&web=1&e=ph73JS&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZyIsInJlZmVycmFsQXBwUGxhdGZvcm0iOiJXZWIiLCJyZWZlcnJhbE1vZGUiOiJ2aWV3In19

## Summary
The Social Media Analyzer application has achieved the following functionalities:
- Automatically read posts.csv file to initialize post into database
- Displaying menu on console
- Reading user input to run the respective functionalities displayed on menu
- Adding new post into the database along with its details include id, content, author, likes, shares and date-time
- Delete existing post from the database using the provided ID
- Retrieveing an existing post using the provided ID
- Retrieveing the top N posts with most likes using the provided number of post to be display
- Retrieveing the top N posts with most shares using the provided number of post to be display
- Quiting the application
- Validating user input to get the correct input's type or format to be stored into post, or to run the respective functionalities. The following methods are implement to achieve this objectives:
  - Method to read user's menu option string input and validate the parsed integer format in order to return the valid parsed integer that correspond to the menu options available.
  - Method to read user's post ID input and call readInputNonNegativeInt to validate the parsed integer format and check if post ID already existed in database in order to return the non-exist post ID integer.
  - Method to read user's string input and validate the parsed integer format in order to return the valid non-negative parsed integer.
  - Method to read user's string input and validate the string format in order to return the valid string.
  - Method to read post's content input and validate the content format in order to return the valid content.
  - Method to read user's string input and validate the parsed integer format in order to return the valid positive parsed integer.
  - Method to read post's date-time input and validate the date-time format in order to return the valid date-time.
  - Method to check if integer is negative to throw user-defined InvalidNegativeIntegerException
  - Method to check if content contains "," to throw user-defined InvalidContentException
  - Method to check if input is empty to throw user-defined EmptyContentException
  - Method to check if integer is negative or zero to throw user-defined InvalidNegativeIntegerException

## Class Design
- ```Main```: Entry point for the Social Media Analyzer application.
- ```SocialMediaAnalyzer```: Main application of the Social Media Analyzer, and includes functionalities to add, delete, retrieve posts, retrieve the top N posts with most likes or shares, and quit. Post initiliazation from posts.csv is automatically run here.
- ```PostDatabase```: Maintains the postDatabase ArrayList and provides operations including create, remove, get, search and sort posts and printing Top N Likes/Shares Post in the console.
- ```Post```: Serves as a Post object with properties include id, content, author, likes, shares and date-time with getter methods to access the private instance variables.
- ```ExistedPostIDException```: User-defined exception for invalid post ID integer.
- ```EmptyInputException```: User-defined exception for empty string.
- ```InvalidContentException```: User-defined exception for string content with "," included.
- ```InvalidNegativeIntegerException```: User-defined exception for negative integer.
- ```InvalidNonPositiveIntegerException```: User-defined exception for non-positive integer.
- ```SocialMediaAnalyzerTest```: Utilizes JUnit4 to create test cases for methods in SocialMediaAnalyzer class.
- ```PostDatabaseTest```: Utilizes JUnit4 to create test cases for methods in PostDatabase class.

## Running From Comment Line

# Important: Please set file path for posts.csv in PostDabase.java before running!!!

1) Go to SocialMediaAnalyzer\src\analyzer directory. Type:
```
cd SocialMediaAnalyzer\src\analyzer
```
2) Compile all .java file. Type:
```
javac *.java
```
3) Go back to SocialMediaAnalyzer directory (the main folder). Type:
```
cd ../..
```
You should be now in SocialMediaAnalyzer.

4) Run Main.java file. Type:
```
java -cp ./src analyzer.Main
```
5) The Social Media Analyzer application is now running.

Here's an example on Windows Command Prompt
```
SocialMediaAnalyzer\src\analyzer>javac *.java
SocialMediaAnalyzer\src\analyzer> cd ../..
SocialMediaAnalyzer>java -cp ./src analyzer.Main
```
