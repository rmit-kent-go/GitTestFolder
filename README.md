# Social Media Analyzer

## Summary


## Class Design
- ```Main```: Entry point for the Social Media Analyzer application.
- ```SocialMediaAnalyzer```: Main application of the Social Media Analyzer, and includes functionalities to add, delete, retrieve posts, retrieve the top N posts with most likes or shares, and quit.
- ```PostDatabase```: Maintains the postDatabase ArrayList and provides operations including create, remove, get, search and sort posts and printing Top N Likes/Shares Post in the console.
- ```Post```: Serves as a Post object with properties include id, content, author, likes, shares and date-time with getter methods to access the private instance variables.
- ```EmptyInputException```: User-defined exception for empty string.
- ```InvalidContentException```: User-defined exception for string content with "," included.
- ```InvalidNegativeIntegerException```: User-defined exception for negative integer.
- ```InvalidNonPositiveIntegerException```: User-defined exception for non-positive integer.
- ```SocialMediaAnalyzerTest```: Utilizes JUnit4 to create test cases for methods in SocialMediaAnalyzer class.
- ```PostDatabaseTest```: Utilizes JUnit4 to create test cases for methods in PostDatabase class.

## Running From Comment Line
```

```
