# Hello World! Assignment


## Summary
This is a sample assignment created in aims of familiarizing yourself with the Oracle we will provide you in JAR form for every assignment.

Follow the instructions in Sakai for Assignment 0 for what to turn in. We will grade this one for you as an example, although it is worth 0 points towards your course grade. Our goal is to head off confusion and problems with the procedure we will follow for coding assignments... to get you familiar with it ASAP.


## Notes about the Oracle
The "Oracle" is meant to be a guide provided to you to see if your program passes some basic test cases, but more importantly is structured in a way that the REAL grading program can grade the submitted program. There will be things tested in the real graded that are possibly not in the Oracle, so we recommend that you develop your own tests in addition to the ones we provide you. Just because you get 100 on the Oracle does NOT guarantee 100 on the assignment! Note that in each assignment we will also provide specific zipping instructions. This is super important, as an incorrectly zipped program cannot be recognized by the grading software. You MUST have your package names as shown in the specification section of the prompt.


## Specifications
In each assignment, we will provide you with an interface to implement, for uniformity's sake. In this assignment, It will be a simple (and perhaps unnecessary) Hello World Interface. If you were submitting this assignment, you would be required to submit this interface as well as your other java files.

## (1) Interface HelloWorld_Interface
package Assignment0;
/**
 * COMP 410
 *
 * Make your class and its methods public!
 * Don't modify this file!
 * Begin by creating a class that implements this interface.
 *
*/

public interface HelloWorld_Interface {
  /*
    Interface: A HelloWorld will implement the following interface

    String say_it
      in: nothing
      return: String "hello world"
        
  String say_it_loud
    in: nothing
    return: String "HELLO WORLD"
  
  */


  String say_it();
  String say_it_loud();
}
## (2) Class HelloWorld
package Assignment0;
public class HelloWorld implements HelloWorld_Interface {


  public HelloWorld ( ) { // default constructor
    // explicitly include this
    // we need to have the default constructor
    // if you then write others, this one will still be there
  }
  
  // rest of your code to implement the various operations
}
## (3) Class RunTests
package Assignment0;
import gradingTools.comp410s20.assignment0.testcases.Assignment0Suite;

public class RunTests {
  public static void main(String[] args){
    Assignment0Suite.main(args);
  }
}
