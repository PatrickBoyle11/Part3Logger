# Part3Logger
1.	In the logger.properties file it has different specification for console logging and file logging. For example, the level is INFO for console handler and ALL for file handler. So, depending on the message it might appear in one and not the other.
2.	This message appears in the logger.log file. It uses ConditionEvaluationResult which was added in JUnit5 and has a message with reasoning why it was disabled.
3.	It is used to assert when a specified exception should be thrown. We can use it when we want to test throwing of exceptions in methods.
4.	TestException
a.	For serializable classes serialVersionUID is used to specify what version of a class is being used so when we want to either serialize or deserialize we are using the right version of the class. Since Exception classes are serializable, we should have a serialVersionUID.
b.	We override it to get the functionality specified, instead of the functionality from the Exception class we are extending.
c.	We don’t override other methods because there is no need. Just like any other class that extends another class we would like to only override the methods we desire to have different outcomes.
5.	It starts running when the class gets initialized and can be used to initialize static variables. When the class gets initializes it fetches the logger.properties file so the Logger Manager can get its rules. Logger is static.
6.	They both use markdown syntax to get the format of the text. In bitbucket you can use markdown for controls with pull and for README.md files.
7.	The test is failing because it runs into the if statement which throws an exception that is then caught, so it misses where timeNow is specified with current millis. So, when it then is run through finally it is still null, thus creates a NullPointerException.
8.	Since the code never accounted for the value of Time Now in the scenario when we get a Timer Exception the finally block throws a null pointer exception which is the one that is used and TimeException gets lost.
9.	Done
 
10.	I’m confused what I’m supposed to submit here-Done
 
11.	Exceptions:
a.	NullPointerException falls under the category of RuntimeException.
b.	TimerException falls under the category of ExceptionClass
c.	 
12.	https://github.com/PatrickBoyle11/Part3Logger
