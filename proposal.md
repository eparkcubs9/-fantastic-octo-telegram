# InterFace Your Problems

See https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet#code for tips on using *Markdown* tags to format __.md__ files

## Goal
 
Work as a team to create a project proposal for your X-team to complete together.
The project does not have to be extremely difficult,
but there must be work to do for each member of your team.
You may reference figures using "See figure 1".  
Be sure to submit corresponding image files, i.e. figure1.png (or figure1.jpg) for each figure.
 
## Grading: To earn full credit, your team's proposal must include:
 
* (md) documentation: [this file] describing purpose and use of your program
 
* Description of a program that has:
 
  ** a main Java program class in a file named Main.java
  
  ** a custom data structure designed and built by your team
  
  ** comprehensive testing of individual units
  
 Caution: You are not being asked to implement this program, at least not yet. 
 We just want your group to make a proposal or pitch for your program.
 
 Tip: Your custom data structure can be composed of or extensions of data structures that you have learned and used in previous programming assignments.  We're looking for decisions about how to build a high-level data structure that will likely have lower-level components.
 
## Problem Description
A program that categorizes assignments by class but also allows the user to weight assignments in that class by their current importance. Hopefully this would allow the user to visualize what assignments they should be working on and drive them to complete those assignments
## Questions to answer for Exercise #2
1. Name: Give your project proposal a name (and edit the top line of this file)
interFace your problems 
2. Output: Describe the output your program will produce.  Include and example format of the output produced. 
The output of the program would be the full list of the assignments that the user puts in, in order of what should be done first.
 
 
Example:
X-Team Activity 2b - Weight 10
Project 3 - Weight 8
Math Hw 2 - Weight 7
...
3. Input: Describe the data that is needed to solve your problem. Include an example format of the input data.
Class Data:
Name, Total number of points, Credits
Assignment Data:
Assignment Name, Due Date, Class, Points Worth, Hours it will take
Example:
*CS, 1000, 3 (Class Data)
*HW 2, 10/31/18, CS, 30, 6 (Assignment Data)
 
4. User Interface: Describe a user interface for your program.  Use text menus or a simple graphic user interface.
We will first import our classes which will be saved into our system. The user will be prompted for the number of classes they are taking, and then will be prompted that number of times for class information.


We will then allow the user to import any assignments they have and information associated with each assignment.
Then user will indicate that they are done inputting assignments and the ordered list will appear.
The user will then have the option to remove assignments using certain keywords and insert new assignments using others.
 
5. Types List: Break your solution idea down into units that you think can be implemented with a single class.
Class class - stores information about each of the users school classes. (Number of points, name, credits)
Assignments class - stores information about each assignment (name, class, due date, etc.) in a hash table.This will be a node in our weighted graph. The weight will be calculated using this information.
Assignments weighted graph - Contains all of the assignments weighted nodes.
 
Name each interface or class and briefly describe its function or purpose.
AssignmentGraph is the interface for our graph class. We want an insert a delete a print and a toString method for this interface. 
We will have a class for each Class, which has all of the information for each class that the user is taking. The class name for this class will be ScheduledClass
We will have a node which has all of the assignments information that the user will input. This class will be called Assignment. 
Our Main class will have all of the prompts for the user and will create all of the objects in our Assignment Graph, and allow the user to visualize the order they should complete their assignments.
We will test all of the functions in our AssignmentGraph interface and in each of our classes. We will use both j-unit tests and black box testing to test the program as well as have also include unit testing to test functionality. 
