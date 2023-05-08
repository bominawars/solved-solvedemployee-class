Download Link: https://assignmentchef.com/product/solved-solvedemployee-class
<br>
iLab 2 of 7: Employee Class We begin our investigation of object-oriented programming by creating an object-oriented program with a class called Employee. You will create two objects based on the Employee class, along with a class that contains the main method. The attributes, constructors, and methods for this class must satisfy the requirements in Steps 1 through 3. After you create the objects, you will prompt the user for information and then display it. We will want to ensure that this first class is well-constructed and tested since we will extend this class in Labs 3 through 6. Due this week: Capture the Console output window and paste into a Word Document. Zip the project folder. Put the zip file and screen shots (Word document) in the Dropbox. Analyze and understand the object UML diagram, which models the structure of the program. The first section specifies the attributes. The second section specifies the operations, and the first character specifies the access modifier value, where: “-” means that the class member is private “+” means that the class member is public. Each attribute has a default value assigned, and you will create private class constants to hold these values and initialize the values in the default constructor. The InputUtitlities and ApplicationUtilities classes are provided for you (see below) and are used by the Main method to display the standard application information and there are methods that will prompt, retrieve, and convert each of the different input data types. You will use these classes for each of the following weeks assignments. Directions on how to include these in your project are provided below. One final note, for this lab ONLY will the attributes be made public. When we discuss accessors and mutators (get and set) methods in Week 3 we will modify these attributes to be “private” and all access to these attributes will be done with the get and set methods, or properties. Layer/Tiered Program Architecture In your following courses you will learn about a design principle called Tiered or Layered Architecture. This is a design technique that professional program desigers use to manage the complexity of real world applications. We do not want to go into the details of a tiered design in this course, but we do want tolearn to program using the underling principles since using the tiered approach is a practical way to simpify the coding process that professional programmers use and you will discover the tiered approach enables us to make changes to an existing program much easier. The programming labs in this course will lead you through this process but let’s define the two standard tiers that we will Print Connect to the iLab here. Submit your assignment to the Dropbox located on the silver tab at the top of this page. (See the Syllabus section “Due Dates for Assignments &amp; Exams” for due dates.) i L A B O V E R V I E W Scenario and Summary Deliverables i L A B S T E P S STEP 1: Understand the UML Class Diagram Back to Top iLab https://devry.equella.ecollege.com/file/dbde261e-a72c-4c54-977b-0ebe3… 1 of 6 5/14/2016 8:35 PM use in this course. Presentaiton tier contains all the classes that will provide input/output operations and the main program. There should NOT be any actual data processing in the presentation tier and the presenation tier should only provide input/ouput operations and execution control. Once data is collected in the presentation tier it is passed into the logic tier for processing. Once the logic tier processes the data the logic tier passes the information back to the presentation tier for output. 1. Logic tier contains all the classes that represent the business objects that are necessary to hold and process the application data. There should not be any user input/output operations in the Logic Tier and the Logic Tier should only process the data collected by operations in the presentation tier and then send the back the information operations in the presentation tier for display. 2. One last note. A tiered design is a “logical” design concept, which means that the physical files that hold the classes can exist in any location within your project. However, MS Visual Studio Solution Explorer provides tools to create folders and subfolders within your project that will allow us to store the classes for each teir into separate folders. However, will will NOT create these folders until Week 4 when we start adding more classes to the application. So, for now we just want to put the various files under the root project folder. In the Week 1 lab you created a set of re-useable classes and methods and in order to demonstrate the power of re-usablity and to provide a common interface in all our programs, you will create a project and add some existing classes that contain re-useable methods that we will use throughout the rest of labs. In order to re-use the existing classes follow these steps: Download the Utility Classes file, which is a zip file that contains two classes (1) ApplicationUtilities.cs and (2) InputUtilities.cs. Unzip the two files and place the files in a known location. 1. 2. Create a new project called “CIS247_WK2_Lab_LASTNAME”. An empty project will then be created. 3. Right click the project name in the Solution Explorer, or select the Project Menu, and select “Add Existing Item” Image Description STEP 2: Create a New Project and Add Existing Classes Back to Top iLab https://devry.equella.ecollege.com/file/dbde261e-a72c-4c54-977b-0ebe3… 2 of 6 5/14/2016 8:35 PM Navigate to the folder where you saved the (1) ApplicationUtilities.cs and (2) InputUtilities.cs class files, select the files, and then click add. 4. 5. The files will be added to your project. The final step is to change the name of the Namespace so all the classes in the project can recognize each other (there are advanced ways around this, but for this course may be easiest to change the namespace. In order to make it easier for the follow on weeks, change the namespace to all the classes to “Employee”. The file list in the Solution Explorer will then look something like: 6. iLab https://devry.equella.ecollege.com/file/dbde261e-a72c-4c54-977b-0ebe3… 3 of 6 5/14/2016 8:35 PM Since all the lab assignments through the rest of the course will re-use classes from the previous week’s assignments, make sure you become proficient in adding existing items–it will reduce the amount of “busy work” you have to do each week! Be sure you follow proper commenting and programming styles (header, indentation, line spacing, etc.) that are specified in the Programming Conventions and Standards guide. Using the provided Class Diagram as a guide code the Employee class in the new project (i.e., “Realize the UML Class diagram”). 1. Add a new class called “Employee” to the project 2. Create private variables and correctly initialize them for the Employee class attributes. Create constants in the Employee class for the default values, and the default constuctor shall set these default values to the appropriate attribute. 3. The multi-argument constructor (parameterized constructor) should initialize all of the attributes using values passed in through the parameter list. 4. As mentioned above, for this lab ONLY will the attributes be made “public” and we will access the attributes directly. Begininning in Week 3 ALL variable attributes of every class will be private and access will be done through the get and set methods. 5. The CalculateWeeklyPay( ) method of the Employee class should return the value of annual salary divided by 52 (return annualSalary / 52;). 6. Most classes will have a ToString method that collects the key class attributes into a single well formated string. The method will always be declared using the “override” keyword (this will be explained in Week 5) and the declaration of the ToString method for every class will look like the following: 7. The ToString method will always return a string value that collects the key attributes, the following shows one technique that you can use to collect the information and return the formatted string: 8. STEP 3: Code the Employee class Back to Top public override string ToString() public override string ToString() { string output; iLab https://devry.equella.ecollege.com/file/dbde261e-a72c-4c54-977b-0ebe3… 4 of 6 5/14/2016 8:35 PM In order to print out currency values in currency format (dollars and cents) you can use the ToString method that each numeric variable has predefined. For example, to output the annualSalary in currency you would use the following: 9. In the Main class, create code statements that perform the following operations. Remember, to access a public method (method or property) of an object, or class, use the DOT notation: For example, to access the DisplayApplicationInformation of the ApplicationUtilities class, the statement would look something like: 1. Display the program information. 2. Create an Employee object using the default constructor. Prompt for and then set the first name, last name, gender, dependents, and annual salary. Remember to use the appropriate methods in the InputUtilties class to prompt for and retreive the values. 3. 4. Display the employee information. Create a second Employee object using the multi-argument constructor using data of your choosing that is the correct type and within the valid ranges for each of the attributes. 5. 6. Display the Employee information for the second employee object. 7. Terminate the application When done, compile and execute your code. Debug errors until your code is error-free. Check your output to ensure that you have the desired output, modify your code as necessary, and rebuild. The following shows some sample output, but your output may look different. } output = “============ Employee Information ============”; output += “Name: ” + firstName + ” ” + lastName; //rest of method omitted return output; output += “Annual Salary: ” + AnnualSalary.ToString(“C2”); STEP 4: Code the Main Program Back to Top objectName.MethodName() ApplicationUtilities.DisplayApplicationInformation(); STEP 5: Compile and Test Back to Top iLab https://devry.equella.ecollege.com/file/dbde261e-a72c-4c54-977b-0ebe3… 5 of 6 5/14/2016 8:35 PM Capture the Console output window and paste it into a Word Document. Put the zip file of you project folder and screen shots (Word document) in the Dropbox. Submit your lab to the Dropbox located on the silver tab at the top of this page. For instructions on how to use the Dropbox, read these step-by-step instructions or watch this Dropbox Tutorial. See the Syllabus section “Due Dates for Assignments &amp; Exams” for due date information. Image Description STEP 6: Submit Deliverables Back to Top Back to Top iLab https://devry.equella.ecollege.com/file/dbde261e-a72c-4c54-977b-0ebe3… 6 of 6 5/14/2016 8:35 PM