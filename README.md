# JavaGUI
 
Java Test Driven Development (TDD) project to exercise Java Graphical User Interface (GUI) App with unit testing ( with **JUnit** )

<img src="./images/GoneFishing_play.png" width="35%" alt="gone fishing!" style="margin:auto;">


<details id="source">
  <summary>Source</summary>

 <em>derived from CISC191GUI</em><br>
 
![220px-MesaLogo](https://github.com/schougaard/SanDiegoMesaCISC191ProgrammingChallenges/assets/716243/334f6724-6afa-4198-9eff-7c49c472cd35)

# San Diego Mesa College CISC 191 Programming Challenges
Programming challenges for San Diego Community College CISC 191 Intermediate Java classes.

Created by
- Professor Dr. Tasha Frankie
- and Professor [Allan Schougaard](https://github.com/schougaard), San Diego Mesa College.

With contributions from: 
- Dom David,
- [Dan Sullivan](https://github.com/uid100)

[source](#source)
<hr />
</details>

<details id="overview">
 <summary>Assignment Overview</summary>

In this assignment you will implementing a simple fishing game that will have you explore many of the most common widgets in the Java Swing library. You will also be asked to consider coding the connection between the GUI and the code behind the scenes using the model-view-controller software design pattern.

This assignment is a little different.

In addition to ensuring the unit tests all pass, and be sure that all the User Stories are implemented.

The tested portion of this programming assignment is very short. The majority of the work will be on creating the GUI and implementing the stories where you will work directly with the GUI rather than the tester file.

  <details id="api">
   <summary>Java APIs</summary>
   
Learning Java APIs can help you develop a variety of skills, including:
 - **Problem-solving skills:** Java APIs provide a wide range of functionality that can be used to solve a variety of problems. Learning how to use Java APIs effectively will help you develop your problem-solving skills.
 - **Analytical skills:** When using Java APIs, you need to be able to understand the documentation and identify the appropriate classes and methods to use. This will help you develop your analytical skills.
 - **Design skills:** Java APIs can be used to design and implement complex applications. Learning how to use Java APIs effectively will help you develop your design skills.
 - **Coding skills:** Java APIs are written in Java, so learning how to use them will help you improve your Java coding skills.
 - **API development skills:** Once you have a good understanding of how to use Java APIs, you can start to develop your own APIs. This is a valuable skill that can make you more marketable to employers.

In addition to these general skills, learning specific Java APIs can also help you develop specific knowledge and expertise. For example, learning the JDBC API can help you develop expertise in database programming. Learning the Swing API can help you develop expertise in GUI development. And learning the Java EE APIs can help you develop expertise in enterprise application development.

Overall, learning Java APIs is a great way to develop your skills and make yourself a more valuable developer.

 </details>
 <details id="swing">
  <summary>Swing</summary>
  
Java Swing is a GUI widget toolkit for Java. It is part of Oracle's Java Foundation Classes (JFC) - an API for providing a graphical user interface for Java programs. Swing was developed to provide a more sophisticated set of GUI components than the earlier Abstract Window Toolkit (AWT). Swing components are platform-independent, meaning that they will look and behave the same on any platform that supports Java. Swing components are also lightweight, meaning that they do not consume a lot of system resources. Swing provides a wide variety of GUI components, including buttons, labels, text fields, menus, tables, and trees. Swing also supports a pluggable look and feel, which allows you to change the appearance of your Swing application without having to rewrite any code. Java Swing is a popular choice for developing graphical user interfaces for Java applications. It is used to develop a wide variety of applications, including desktop applications, web applications, and mobile applications.
  
  </details>
  
[overview](#overview)

<hr />
</details>

<details id="setup">
 <summary>Setup</summary>
    
1. From the <> Code dropdown link in the repository (above), download the Zip file to your computer.
2. Extract the files to your working folder
3. Open Eclipse and import the project.
   - You can use File>Import menu item or right-click in the Package Manager and choose Import.
   - Select General>Projects from Folder or Archive
   - Navigate into the project until you see the `bin` and `src` folders, and choose _open_
4. Expand the project in the package explorer and find the `.java` files below the `src` folder.

 [setup](#setup)
 <hr />
</details>

<details id="code-layout">
 <summary>Code Layout</summary>
 
You are going to make a game about fishing, and a low-fidelity rending of the GUI looks like this:

![Gone Fishing game in starting state.](images/GoneFishing_start.png)

The game is played by clicking on the buttons in the middle of the window:

![Gone Fishing game in partially played state.](images/GoneFishing_play.png)

The layout of this project is similar to the the java classes lab. You will implement the logic of several java classes and interfaces.

When the player clicks on a location without fish, the button turns into an icon indicating empty, and the number of tries is reduced. When the player clicks on a location with a school of fish, the button displays a fish icon, and the number of tries and the number of fish remaining are both reduced.

When the last fish has been caught or the last try has been used the game is over:

![Gone Fishing game when fishes win.](images/GoneFishing_done.png)

There are 3 main files you will edit in this programming assignment: `FishingButton`, `FishingButtonListener`, and `GoneFishingView`.

### FishingButton
The buttons for the "fishing" portion of this mini-game.

### FinishButtonListener
This will help handle the events and actions dealing with clicking the buttons.

### GoneFishingView
This is where you will add all the components that the users will see.

[code-layout](#code-layout)
 <hr />
</details>

<details id="programming-tasks">
 <summary>Programming Tasks</summary>

1. Make sure all unit tests all pass, **and**
2. All the **User Stories** are implemented.

The tested portion of this programming assignment is very short. The majority of the work will be on creating the GUI and implementing the stories where you will work directly with the GUI rather than the tester file.


<details>
 <summary>User Stories</summary>
 
Implement the following user stories **one by one** in the order given. If you need additional help, see **Programming Tasks** for more detailed descriptions. 
1. As a computer user, I can see a window with the title "Gone Fishing" so I can see what program I am running.
2. As a computer user, when I click on the X in the top corner of the window, the program exits.
3. As a computer user, I can see instructions in the window.
4. As a computer user, I can see who programmed the game.
5. As a computer user, I can see the grid where the game is played. The grid is 6 by 6 buttons.
6. As a computer user, when I start the program, I can see all the UI widgets in the game.
7. As a player, I can see how many tries I have left on a slider, so I can see if I am winning. I start with 30 tries.
8. As a player, I can see how many schools of fish are left on a slider, so I can see if the fish are winning. The game starts with 10 schools of fish.
9. When I click on a button in the grid, it shows me if I caught a fish or not, so I can see my fishing skills.
10. When I click on a button in the grid, I cannot click on it again, so I cannot cheat.
11. When I click on a button, the number of tries goes down by one.
12. When I click on a button, and I caught a school of fish, the number of schools of fish goes down by one.
13. If I manage to catch all the fish before I run out of tries, I get a message: "Game Over - You Win!" and the program exits.
14. If I run out of tries before I have caught all the fish, I get a message: "Game Over - Fishes Win!" and the program exits.

</details>

<details>
  <summary>testGoneFishingButton</summary>

 - The buttons in the GUI will keep track of their row-col position in the grid.
   - Add the required instance variables (fields) to keep track of this information.
 - Complete the constructor to initialize the instance variables (fields)
 - Add the two getters to be able to get the row and column position of a FishingButton

</details>
<details>
  <summary>testGoneFishingView</summary>
  - Add an instance variable (field) in the GoneFishingView for a GoneFishingModel</li>
  - Constructor:
    - Don't forget to assign the model instance variable to the parameter of the constructor
    - Add a title to the JFrame. REMINDER: The class you are in extends [JFrame](https://docs.oracle.com/javase/8/docs/api/javax/swing/JFrame.html) so you have access to ALL public setters in `JFrame`. A GoneFishingView IS-A JFrame. Look through the API if you need reminders on available methods or use Eclipse's auto-suggest features. For example, you can write _**this**_ in the constructor to look through available methods of the JFrame API. The **this** keyword refers to the current instance of the object and the **dot** operator, of course, is how you access methods and public attributes of an object.
    - You'll be working with labels and buttons. Perhaps look through [this example](https://www.javatpoint.com/java-jframe) first to see if you can simply add to the `JFrame` then go back and try to get what you need in this actual programming assignment. The hope is you're at least comfortable adding components to the `JFrame`. Your current trouble should be in placing the components where you want them rather than being too afraid to add any component at all. :)<br />You can run the GoneFishingView class so that you can see what you are adding to the JFrame.
 - At this point, do not worry too much about the tester file and play around with getting widgets to the JFrame. Additional Hints are shown below

</details>
<details>
  <summary>GoneFishingView</summary>
You will have to use layout managers in this assignment so that you can position the components (widgets) on the JFrame where you want them to go. Run this file instead of the tester so that you can check out the GUI. Running the tester will close the GUI automatically thus preventing you from checking your progress on building the user interface.

1. Start by adding a BorderLayout to the main JFrame. Technically this is the default layout for JFrame, but it's being shown here to introduce you to the setLayout method and the creation of a layout manager object.&nbsp;<br />To add a layout, you must instantiate an object of that type (in this case BorderLayout) and then pass it to the setLayout method of the JFrame or JPanel.You can also do this in one line since we don't need to keep track of the instance of the layout manager.
```
this.setLayout(new BorderLayout()); //the this keyword refers to the instance of the GoneFishingView which IS-A JFrame.
```
You may need to import the necessary libraries to use BorderLayout like you have done when adding the other components.</p>
3. Positioning<br />
[BorderLayout diagram](images/positioning.png)<br />
At this point, you now have access to the BorderLayout positions as shown in the image above.
4. Add the first `JLabel` for the _instructions_ and add it to the West side.
```
JLabel instructions = new JLabel("Click on the buttons to fish");<br />this.add(instructions, BorderLayout.WEST);
```
But.... Let's actually add it to a `JPanel` and then add the `JPanel` to the `JFrame`.
If you consider the Gone Fishing preview, you are breaking up the JFrame into different areas that are managed by JPanels.
You will add the components to the `JPanel` and then finally place the `JPanel` in the `JFrame.`
```
JPanel instructions = new JPanel();                                    //Create the JPanel
JLabel instructionLabel = new JLabel("Click on the buttons to fish");  //Create and add the component to the JPanel
instructions.add(instructionLabel);
this.add(instructions,  BorderLayout.WEST)                             //add the JPanel to the JFrame in the WEST location
```

There is an overridden version of `add` where you can specify where to place the element as shown in the code above. 
BorderLayout holds static variables for the locations: `WEST`, `EAST`, `CENTER`, `NORTH`, `SOUTH`

</details>
<details>
  <summary>"fishing"Panel!</summary>

[Gone Fishing game at start of game.](images/GoneFishing_start)
The center of the JFrame holds all the buttons which is where the "fishing" will take place. Clicking on the buttons can lead to revealing a "fish".

1. Create a new `JPanel` and add a ![GridLayout](https://docs.oracle.com/javase%2F7%2Fdocs%2Fapi%2F%2F/java/awt/GridLayout.html) to hold enough buttons that are shown in the programming assignment.
     - When creating a GridLayout, there are two parameters that you pass to set the # of rows and the # of columns of the grid. As you add components to the JPanel, it would fill these "cells" from left to right and top to bottom.
     - Pause. Look at the model class now. Are there variables in this class that you should use that dictates how many buttons you should have in this fishing game? The model holds some instance variables that can be easily updated later if you wanted to alter the number of buttons. Use the model information when creating the buttons (how man
2. Write a nested loop that will allow you to generate the total number of buttons required. The nested loop should resemble a 2D array traversal because you will need the row and column information!
 The row-column information is required because the buttons in the GUI must store their row-column position!
3. Add the fishing buttons to the `JPanel` (not directly to the `JFrame`).</li>
4. Add the `JPanel` object to the center of the `JFrame`.</li>
5. You will revisit this section later to connect the listener class to the buttons so that they perform an action when there is a click event on them.

</details>
<details>
  <summary>SliderPanel</summary>

The instruction label was placed in a `JPanel` that was placed in the `WEST`, and the fishing buttons were placed in a `JPanel` that was then added to the center. What should you do with the Sliders?
 1. Create a JPanel where you will add the sliders</li>
 2. Create a Slider and figure out how to set its properties so that it's vertical and looks like the image in this programming assignment. Look for ways to change the following: maximum, tick spacing, paint ticks, paint labels, enabled/disabled, border
 3. Add a layout manager to the JPanel. What kind should you add?
    **Hint:** _If you want, you can think of that slider section as a 1-by-n grid!_
 4. Add the Sliders and any necessary labels to the JPanel.
 5. Add the JPanel to the JFrame on the EAST side.
 
 </details>
 <details>
  <summary>BottomLabel</summary>
  
 1. Create JPanel to hold the JLabel
 2. Add the JLabel to the JPanel
 3. Add the JPanel to the JFrame in the SOUTH.

At this point, you have put in a lot of work getting the user interface up and going. 
It should roughly resemble the layout in the picture, but some slight changes here and there should be ok. 
The tester does not test that the layout is exactly the same so you have some leeway.

</details>
<details>
  <summary>fishingButtonListener</summary>

#### FishingButtonListener
The FishingButtonListener class will implement the behaviors of an ActionListener. 
It will connect the GUI buttons and the model together when users interact with the fishing panel.

 1. Add the required relationship in the class header so that this class can claim to behave like the ActionListener interface. Import any necessary libraries to use ActionListener.
 2. Once a class implements an interface, it must provide all of the methods that are defined in the interface it implements. Do that now. Recall that Eclipse makes this easy for you by using the first quick fix.
 3. Complete the constructor and be sure to add any required instance variables (fields).
 
 #### actionPerformed()
This is the method that will run when there is a mouse click on the fishing buttons. 
We will now be using the `GoneFishingModel.`
1. Take a moment to do a quick scan of the `GoneFishingModel` which keeps track of the state of our game.
2. Pay special attention to the `fishAt()`
    - What are the formal parameters? 
    - What data does this return?
    - What instance variables does it alter?
3. Comment out the `GoneFishingModel`. You will see that there are `TODO` comments in this file. Take the time now to try to piece together what the model will do for the game.
4. In the actionPerformed method, figure out how to call the model's `fishAt()` method. Where are the actual parameters coming from to use this method?
5. The `fishAt()` method should be in a conditional statement to check if it returns true. Change the text of the button to "fish" if there is a fish, otherwise, it should be "X".
6. Call the GUI class' updateUI method.

#### addActionListener
What you have just completed are the separate code for the button and the listener. 
The `FishingButtonListener` needs to be added as the action listener of the buttons once you have completed the majority of the tasks that the listener will complete.

1. Go back to the view class
2. Look for the area where you created the FishingButton objects.
3. After creating a button, add the actionlistener! The update should look something similar to the code below.

This is the code inside the nested loop from the view constructor
```
//create a FishingButton!
FishingButton fish = new FishingButton(row, col);

//connect the listener
fish.addActionListener( new FishingButtonListener(model, this, fish) );
```

</details>
<details style="margin-bottom: 25px;">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
    <summary style="cursor: pointer;">GoneFishingView-updateUI</summary>

This class has access to the model therefore it always has access to the latest updates. 
Find a way to update the sliders by getting the updated information from the model.

Tidy up the Fishing View. For example, add a minimum dimension so that when you click on the buttons, you do not end up with any ellipses due to the buttons being too small to display the text. You can also play around with styling the buttons if you want to explore further customization!

 </details>

[programming-tasks](#programming-tasks)
 <hr />
</details>

<details id=submission>
 <summary>Submission</summary>

## Complete and zip the project
1. Run and add the code to the src folder until the tests are successful.
2. Uncomment each test case in the **Test** file (`TestAdvancedClasses.java`), one at a time. 
Do not modify the content in this file except to uncomment the tests. Add and modify class files
as needed for the tests to pass.
3. Review and refactor any of the code as needed:
    - be sure your code follows good coding practices and coding style and standards.
    - update the javadoc comments at the top of the file to add your name as author
    - update the comments for each method in the file.
4. Export the project as a zip file and submit your work.
   _Note: You are turning in the Eclipse project so that I can easily open it and run it on my computer._

     [submission](#submission)
 <hr />
</details>

<details>
 <summary>Rubric</summary>

[Rubric](Rubric.md)

</details>


___________

_this repository is a subset of the CISC191 exercises. It is derived from the CISC191ProgrammingChallenges 
activity hosted by Professor Allan Schougaard, San Diego Mesa College, and not a direct fork._

_This project is to decompose that repository into git submodules_
