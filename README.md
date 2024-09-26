# JavaGUI
 
Java Test Driven Development (TDD) project to exercise Java Graphical User Interface (GUI) App with unit testing ( with **JUnit** )

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
[back](#source)
<hr />
</details>
<details>
 <summary>Assignment Overview</summary>
</details>

## Assignment Overview

<div class="enhanceable_content tabs">
    <ul>&nbsp; &nbsp; &nbsp; &nbsp;
        <li><a href="#tab-1">Assignment Overview</a></li>
        &nbsp; &nbsp; &nbsp; &nbsp;
        <li><a href="#tab-2">Setup</a></li>
        &nbsp; &nbsp; &nbsp; &nbsp;
        <li><a href="#tab-3">Code Layout</a></li>
        &nbsp; &nbsp; &nbsp; &nbsp;
        <li><a href="#tab-4">Programming Task(s)</a></li>
        &nbsp; &nbsp; &nbsp; &nbsp;
        <li><a href="#tab-5">Submission</a></li>
        &nbsp; &nbsp;
    </ul>
    <div id="tab-1">
        <p>Learning Java APIs can help you develop a variety of skills, including:</p>
        <div id="collapse1" class="panel-collapse collapse in" aria-expanded="true">
            <div id="summer0" class="panel-body summernote">
                <div class="resize-observable">
                    <div class="markdown markdown-main-panel" dir="ltr">
                        <ul data-sourcepos="3:1-8:0">
                            <li data-sourcepos="3:1-3:219"><strong>Problem-solving skills:</strong> Java APIs provide a wide range of functionality that can be used to solve a variety of problems. Learning how to use Java APIs effectively will help you develop your problem-solving skills.</li>
                            <li data-sourcepos="4:1-4:206"><strong>Analytical skills:</strong> When using Java APIs, you need to be able to understand the documentation and identify the appropriate classes and methods to use. This will help you develop your analytical skills.</li>
                            <li data-sourcepos="5:1-5:172"><strong>Design skills:</strong> Java APIs can be used to design and implement complex applications. Learning how to use Java APIs effectively will help you develop your design skills.</li>
                            <li data-sourcepos="6:1-6:126"><strong>Coding skills:</strong> Java APIs are written in Java, so learning how to use them will help you improve your Java coding skills.</li>
                            <li data-sourcepos="7:1-8:0"><strong>API development skills:</strong> Once you have a good understanding of how to use Java APIs, you can start to develop your own APIs. This is a valuable skill that can make you more marketable to employers.</li>
                        </ul>
                        <p data-sourcepos="9:1-9:389">In addition to these general skills, learning specific Java APIs can also help you develop specific knowledge and expertise. For example, learning the JDBC API can help you develop expertise in database programming. Learning the Swing API can help you develop expertise in GUI development. And learning the Java EE APIs can help you develop expertise in enterprise application development.</p>
                        <p data-sourcepos="11:1-11:110">Overall, learning Java APIs is a great way to develop your skills and make yourself a more valuable developer.<br /><br />Java <span class="citation-0">Swing is a GUI widget toolkit for Java. It is part of Oracle's Java Foundation Classes (JFC) - </span><span class="citation-0 citation-1 citation-end-0">an API for providing a graphical user interface</span><span class="citation-1"> for Java programs. Swing was developed to provide a more sophisticated set of GUI components than the earlier Abstract Window Toolkit (AWT). </span><span class="citation-1 citation-end-1">Swing</span> components are platform-independent, meaning that they will look and behave the same on any platform that supports Java. Swing components are also lightweight, meaning that they do not consume a lot of system resources. Swing provides a wide variety of GUI components, including buttons, labels, text fields, menus, tables, and trees. Swing also supports a pluggable look and feel, which allows you to change the appearance of your Swing application without having to rewrite any code. Java Swing is a popular choice for developing graphical user interfaces for Java applications. It is used to develop a wide variety of applications, including desktop applications, web applications, and mobile applications.<br /><br />In this assignment you will implementing a simple fishing game that will have you explore many of the most common widgets in the Java Swing library. You will also be asked to consider coding the connection between the GUI and the code behind the scenes using the model-view-controller software design pattern.</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <div id="tab-2">
        <div class="panel-body">All of the programming assignments are on the course GitHub repository: <a href="https://github.com/schougaard/CISC191ProgrammingChallenges" target="_blank" rel="noopener">https://github.com/schougaard/CISC191ProgrammingChallenges</a><br />Click on the <strong><i>green &lt;&gt;Code</i></strong> button to download the repo if needed.</div>
    </div>
    <div id="tab-3">
        <h2 style="margin-top: 12px; margin-bottom: 12px; color: #2d3b45; font-family: 'Lato Extended', Lato, 'Helvetica Neue', Helvetica, Arial, sans-serif;">Code Layout</h2>
        <p style="margin-top: 12px; margin-bottom: 12px; color: #2d3b45; font-family: 'Lato Extended', Lato, 'Helvetica Neue', Helvetica, Arial, sans-serif;">You are going to make a game about fishing, and a low-fidelity rending of the GUI looks like this:</p>
        <div><img src="https://sdccd.instructure.com/courses/2441328/files/146951807/preview" alt="Gone Fishing game in starting state." width="708" height="258" data-api-endpoint="https://sdccd.instructure.com/api/v1/courses/2441328/files/146951807" data-api-returntype="File" /></div>
        <div>
            <p style="margin-top: 12px; margin-bottom: 12px; color: #2d3b45; font-family: 'Lato Extended', Lato, 'Helvetica Neue', Helvetica, Arial, sans-serif;">The game is played by clicking on the buttons in the middle of the window:</p>
        </div>
        <div><img src="https://sdccd.instructure.com/courses/2441328/files/146951808/preview" alt="Gone Fishing game in partially played state." width="708" height="258" data-api-endpoint="https://sdccd.instructure.com/api/v1/courses/2441328/files/146951808" data-api-returntype="File" /></div>
        <p><br />The layout of this project is similar to the the java classes lab. You will implement the logic of several java classes and interfaces.</p>
        <div>
            <p style="margin-top: 12px; margin-bottom: 12px; color: #2d3b45; font-family: 'Lato Extended', Lato, 'Helvetica Neue', Helvetica, Arial, sans-serif;">When the player clicks on a location without fish, the button turns into an icon indicating empty, and the number of tries is reduced. When the player clicks on a location with a school of fish, the button displays a fish icon, and the number of tries and the number of fish remaining are both reduced.</p>
            <p style="margin-top: 12px; margin-bottom: 12px; color: #2d3b45; font-family: 'Lato Extended', Lato, 'Helvetica Neue', Helvetica, Arial, sans-serif;">When the last fish has been caught or the last try has been used the game is over:</p>
        </div>
        <div><img src="https://sdccd.instructure.com/courses/2441328/files/146951811/preview" alt="Gone Fishing game when fishes win." width="706" height="258" data-api-endpoint="https://sdccd.instructure.com/api/v1/courses/2441328/files/146951811" data-api-returntype="File" /></div>
        <div>There are 3 main files you will edit in this programming assignment: FishingButton, FishingButtonListener, and GoneFishingView.<br />
            <div>
                <h3>FishingButton</h3>
            </div>
            <div>The buttons for the "fishing" portion of this mini-game.</div>
            <h3>FinishButtonListener</h3>
            <div>This will help handle the events and actions dealing with clicking the buttons.</div>
            <h3>GoneFishingView</h3>
            <div>This is where you will add all the components that the users will see.</div>
            <div><span style="color: #2d3b45; font-family: 'Lato Extended', Lato, 'Helvetica Neue', Helvetica, Arial, sans-serif; font-size: 1.8em;">User Stories</span></div>
            <div>
                <p style="margin-top: 12px; margin-bottom: 12px; color: #2d3b45; font-family: 'Lato Extended', Lato, 'Helvetica Neue', Helvetica, Arial, sans-serif;">Implement the following user stories&nbsp;<strong>one by one</strong>&nbsp;in the order given. If you need additional help, go to the more detailed descriptions on the Programming Task page.</p>
                <ol style="padding: 0px; margin-right: 0px; margin-bottom: 6px; margin-left: 25px; color: #2d3b45; font-family: 'Lato Extended', Lato, 'Helvetica Neue', Helvetica, Arial, sans-serif;">
                    <li>As a computer user, I can see a window with the title "Gone Fishing" so I can see what program I am running.</li>
                    <li>As a computer user, when I click on the X in the top corner of the window, the program exits.</li>
                    <li>As a computer user, I can see instructions in the window.</li>
                    <li>As a computer user, I can see who programmed the game.</li>
                    <li>As a computer user, I can see the grid where the game is played. The grid is 6 by 6 buttons.</li>
                    <li>As a computer user, when I start the program, I can see all the UI widgets in the game.</li>
                    <li>As a player, I can see how many tries I have left on a slider, so I can see if I am winning. I start with 30 tries.</li>
                    <li>As a player, I can see how many schools of fish are left on a slider, so I can see if the fish are winning. The game starts with 10 schools of fish.</li>
                    <li>When I click on a button in the grid, it shows me if I caught a fish or not, so I can see my fishing skills.</li>
                    <li>When I click on a button in the grid, I cannot click on it again, so I cannot cheat.</li>
                    <li>When I click on a button, the number of tries goes down by one.</li>
                    <li>When I click on a button, and I caught a school of fish, the number of schools of fish goes down by one.</li>
                    <li>If I manage to catch all the fish before I run out of tries, I get a message: "Game Over - You Win!" and the program exits.</li>
                    <li>If I run out of tries before I have caught all the fish, I get a message: "Game Over - Fishes Win!" and the program exits.</li>
                </ol>
            </div>
        </div>
    </div>
    <div id="tab-4">
        <h2>Programming Task(s)</h2>
        <p>The tested portion of this programming assignment is very short. The majority of the work will be on creating the GUI and implementing the stories where you will work directly with the GUI rather than the tester file.</p>
        <details style="margin-bottom: 25px;">
            <summary style="cursor: pointer;">testGoneFishingButton</summary>
            <br />
            <div style="border: thin solid #f1f3f4; padding-top: 5px; padding-right: 15px; padding-bottom: 5px;">
                <ul>
                    <li>The buttons in the GUI will keep track of their row-col position in the grid.
                        <ul>
                            <li>Add the required instance variables (fields) to keep track of this information.</li>
                        </ul>
                    </li>
                    <li>Complete the constructor to initialize the instance variables (fields)</li>
                    <li>Add the two getters to be able to get the row and column position of a FishingButton</li>
                </ul>
            </div>
        </details>
        <details style="margin-bottom: 25px;">
            <summary style="cursor: pointer;">testGoneFishingView</summary>
            <br />
            <div style="border: thin solid #f1f3f4; padding-top: 5px; padding-right: 15px; padding-bottom: 5px;">
                <ul>
                    <li>Add an instance variable (field) in the GoneFishingView for a GoneFishingModel</li>
                    <li>Constructor:
                        <ol>
                            <li>Don't forget to assign the model instance variable to the parameter of the constructor</li>
                            <li>Add a title to the JFrame. REMINDER: The class you are in extends <a href="https://docs.oracle.com/javase/8/docs/api/javax/swing/JFrame.html" target="_blank" rel="noopener">JFrame</a> so you have access to ALL public setters in JFrame. A GoneFishingView IS-A JFrame. Look through the API if you need reminders on available methods or use Eclipse's auto-suggest features. For example, you can write <strong><i>this.</i></strong> in the constructor to look through available methods of the JFrame API. The <strong>this</strong> keyword refers to the current instance of the object and the <i><strong>dot</strong></i> operator, of course,&nbsp; is how you access methods and public attributes of an object.</li>
                            <li>You'll be working with labels and buttons. Perhaps look through<a href="https://www.javatpoint.com/java-jframe" target="_blank" rel="noopener"> this example</a> first to see if you can simply add to the JFrame then go back and try to get what you need in this actual programming assignment. The hope is you're at least comfortable adding components to the JFrame. Your current trouble should be in placing the components where you want them rather than being too afraid to add any component at all. :)<br />You can run the GoneFishingView class so that you can see what you are adding to the JFrame.</li>
                            <li>At this point, do not worry too much about the tester file and play around with getting widgets to the JFrame. Additional Hints are shown below</li>
                        </ol>
                    </li>
                </ul>
            </div>
        </details>
        <details style="margin-bottom: 25px;">
            <summary style="cursor: pointer;">GoneFishingView</summary>
            <br />
            <div style="border: thin solid #f1f3f4; padding-top: 5px; padding-right: 15px; padding-bottom: 5px;">
                <p>You will have to use layout managers in this assignment so that you can position the components (widgets) on the JFrame where you want them to go. Run this file instead of the tester so that you can check out the GUI. Running the tester will close the GUI automatically thus preventing you from checking your progress on building the user interface.</p>
                <ol>
                    <li>Start by adding a BorderLayout to the main JFrame. Technically this is the default layout for JFrame, but it's being shown here to introduce you to the setLayout method and the creation of a layout manager object.&nbsp;<br />To add a layout, you must instantiate an object of that type (in this case BorderLayout) and then pass it to the setLayout method of the JFrame or JPanel.You can also do this in one line since we don't need to keep track of the instance of the layout manager. <br />
                        <pre>this.setLayout(new BorderLayout()); //the this keyword refers to the instance of the GoneFishingView which IS-A JFrame.</pre>
                        <p>You may need to import the necessary libraries to use BorderLayout like you have done when adding the other components.</p>
                    </li>
                    <li>Positioning<br /><img src="https://sdccd.instructure.com/courses/2441328/files/146951908/preview" alt="BorderLayout diagram." data-api-endpoint="https://sdccd.instructure.com/api/v1/courses/2441328/files/146951908" data-api-returntype="File" /><br />At this point, you now have access to the BorderLayout positions as shown in the image above.</li>
                    <li>Add the first JLabel for the "instructions" and add it to the West side. <br />
                        <pre>JLabel instructions = new JLabel("Click on the buttons to fish");<br />this.add(instructions, BorderLayout.WEST);</pre>
                        <p>But.... Let's actually add it to a JPanel and then add the JPanel to the JFrame. If you consider the Gone Fishing preview, you are breaking up the JFrame into different areas that are managed by JPanels. You will add the components to the JPanel and then finally place the JPanel in the JFrame.&nbsp;</p>
                        <pre>JPanel instructions = new JPanel();                                    //Create the JPanel<br />JLabel instructionLabel = new JLabel("Click on the buttons to fish");  //Create and add the component to the JPanel<br />instructions.add(instructionLabel);           <br />this.add(instructions,  BorderLayout.WEST)                             //add the JPanel to the JFrame in the WEST location</pre>
                        <p>There is an overridden version of add where you can specify where to place the element as shown in the code above. BorderLayout holds static variables for the locations: WEST, EAST, CENTER, NORTH, SOUTH</p>
                    </li>
                </ol>
            </div>
        </details>
        <details style="margin-bottom: 25px;">
            <summary style="cursor: pointer;">"fishing"Panel!</summary>
            <br />
            <div style="border: thin solid #f1f3f4; padding-top: 5px; padding-right: 15px; padding-bottom: 5px;">
                <p><img src="https://sdccd.instructure.com/courses/2441328/files/146951912/preview" alt="Gone Fishing game at start of game." data-api-endpoint="https://sdccd.instructure.com/api/v1/courses/2441328/files/146951912" data-api-returntype="File" /></p>
                <p>The center of the JFrame holds all the buttons which is where the "fishing" will take place. Clicking on the buttons can lead to revealing a "fish".</p>
                <ol>
                    <li>Create a new JPanel and add a <a href="https://docs.oracle.com/javase%2F7%2Fdocs%2Fapi%2F%2F/java/awt/GridLayout.html" target="_blank" rel="noopener">GridLayout</a> to hold enough buttons that are shown in the programming assignment. When creating a GridLayout, there are two parameters that you pass to set the # of rows and the # of columns of the grid. As you add components to the JPanel, it would fill these "cells" from left to right and top to bottom. <br />Pause. Look at the model class now. Are there variables in this class that you should use that dictates how many buttons you should have in this fishing game? The model holds some instance variables that can be easily updated later if you wanted to alter the number of buttons. Use the model information when creating the buttons (how many).&nbsp;</li>
                    <li>Write a nested loop that will allow you to generate the total number of buttons required. The nested loop should resemble a 2D array traversal because you will need the row and column information!<br />The row-column information is required because the buttons in the GUI must store their row-column position!</li>
                    <li>Add the fishing buttons to the JPanel (not directly to the JFrame).</li>
                    <li>Add the JPanel object to the center of the JFrame.</li>
                    <li>You will revisit this section later to connect the listener class to the buttons so that they perform an action when there is a click event on them.</li>
                </ol>
            </div>
        </details>
        <details style="margin-bottom: 25px;">
            <summary style="cursor: pointer;">SliderPanel</summary>
            <br />
            <div style="border: thin solid #f1f3f4; padding-top: 5px; padding-right: 15px; padding-bottom: 5px;">
                <p>The instruction label was placed in a <span style="font-family: 'Courier New';">JPanel</span> that was placed in the WEST, and the fishing buttons were placed in a JPanel that was then added to the center. What should you do with the Sliders?</p>
                <ol>
                    <li>Create a JPanel where you will add the sliders</li>
                    <li>Create a Slider and figure out how to set its properties so that it's vertical and looks like the image in this programming assignment. Look for ways to change the following: maximum, tick spacing, paint ticks, paint labels, enabled/disabled, border</li>
                    <li>Add a layout manager to the JPanel. What kind should you add? Hint: If you want, you can think of that slider section as a 1-by-n grid!</li>
                    <li>Add the Sliders and any necessary labels to the JPanel.</li>
                    <li>Add the JPanel to the JFrame on the EAST side.</li>
                </ol>
            </div>
        </details>
        <details style="margin-bottom: 25px;">
            <summary style="cursor: pointer;">BottomLabel</summary>
            <br />
            <div style="border: thin solid #f1f3f4; padding-top: 5px; padding-right: 15px; padding-bottom: 5px;">
                <ol>
                    <li>
                        <div class="panel-body">
                            <ol>
                                <li>Create JPanel to hold the JLabel</li>
                                <li>Add the JLabel to the JPanel</li>
                                <li>Add the JPanel to the JFrame in the SOUTH.</li>
                            </ol>
                            <p>At this point, you have put in a lot of work getting the user interface up and going. It should roughly resemble the layout in the picture, but some slight changes here and there should be ok. The tester does not test that the layout is exactly the same so you have some leeway.</p>
                        </div>
                    </li>
                </ol>
            </div>
        </details>
        <details style="margin-bottom: 25px;">
            <summary style="cursor: pointer;">fishingButtonListener</summary>
            <br />
            <div style="border: thin solid #f1f3f4; padding-top: 5px; padding-right: 15px; padding-bottom: 5px;">
                <p>The FishingButtonListener class will implement the behaviors of an ActionListener. It will connect the GUI buttons and the model together when users interact with the fishing panel.</p>
                <ol>
                    <li>Add the required relationship in the class header so that this class can claim to behave like the ActionListener interface. Import any necessary libraries to use ActionListener.</li>
                    <li>Once a class implements an interface, it must provide all of the methods that are defined in the interface it implements. Do that now. Recall that Eclipse makes this easy for you by using the first quick fix.</li>
                    <li>Complete the constructor and be sure to add any required instance variables (fields).</li>
                </ol>
                <p>actionPerformed</p>
                <p>This is the method that will run when there is a mouse click on the fishing buttons. We will now be using the GoneFishingModel.</p>
                <ol>
                    <li>Take a moment to do a quick scan of the <span style="font-family: 'Courier New';">GoneFishingModel</span> which keeps track of the state of our game.</li>
                    <li>Pay special attention to the <span style="font-family: 'Courier New';">fishAt </span>method.<br />What are the formal parameters? <br />What data does this return? What instance variables does it alter?</li>
                    <li>Comment out the <span style="font-family: 'Courier New';">GoneFishingModel</span>. You will see that there are TODO comments in this file. Take the time now to try to piece together what the model will do for the game.</li>
                    <li>In the actionPerformed method, figure out how to call the model's fishAt method. Where are the actual parameters coming from to use this method?</li>
                    <li>The fishAt method should be in a conditional statement to check if it returns true. Change the text of the button to "fish" if there is a fish, otherwise, it should be "X".</li>
                    <li>Call the GUI class' updateUI method.<br /><br /></li>
                </ol>
                <p>&nbsp;</p>
                <p>addActionListener</p>
                <p>What you have just completed are the separate code for the button and the listener. The FishingButtonListener needs to be added as the action listener of the buttons once you have completed the majority of the tasks that the listener will complete.</p>
                <ol>
                    <li>Go back to the view class</li>
                    <li>Look for the area where you created the FishingButton objects.</li>
                    <li>After creating a button, add the actionlistener! The update should look something similar to the code below. <br />
                        <pre><span style="background-color: #ffff00; color: #000000;">This is the code inside the nested loop from the view constructor	<br /></span><br /> //create a FishingButton!<br />  FishingButton fish = new FishingButton(row, col);<br />				<br />  //connect the listener<br />  fish.addActionListener( new FishingButtonListener(model, this, fish) );</pre>
                    </li>
                </ol>
            </div>
        </details>
        <details style="margin-bottom: 25px;">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
            <summary style="cursor: pointer;">GoneFishingView-updateUI</summary>
            <br />
            <div style="border: thin solid #f1f3f4; padding-top: 5px; padding-right: 15px; padding-bottom: 5px;">
                <ul>
                    <li>
                        <p>This class has access to the model therefore it always has access to the latest updates. Find a way to update the sliders by getting the updated information from the model.&nbsp;</p>
                        <p>Tidy up the Fishing View. For example, add a minimum dimension so that when you click on the buttons, you do not end up with any ellipses due to the buttons being too small to display the text. You can also play around with styling the buttons if you want to explore further customization!</p>
                    </li>
                </ul>
            </div>
        </details>
    </div>
    <div id="tab-5">
        <p>To turn in your project:</p>
        <ol>
            <li>Comment your code even if you are not 100% sure yet. You will receive feedback and be able to fix any issues for resubmissions.</li>
            <li>Export your project (as explained in <a id="140787516" class="instructure_file_link instructure_scribd_file inline_disabled" href="https://sdccd.instructure.com/courses/2441328/files/140787516?wrap=1" target="_blank" rel="noopener" data-canvas-previewable="true" data-api-endpoint="https://sdccd.instructure.com/api/v1/courses/2441328/files/140787516" data-api-returntype="File"><span class="instructure_file_holder link_holder instructure_file_link_holder">HowToSubmitEclipseProject.docx</span></a></li>
            <li>Make sure your project has your name on it first! Right-click on the project in Eclipse under package explorer then <strong>refactor-&gt;rename</strong>
                <ol>
                    <li>Your exported Eclipse project that should have been renamed prior to exporting it as a zip. Remember you are adding your name at the end of the project name.</li>
                    <li>Every java source file that was you edited to pass the JUnit test or mentioned in the programming assignment specification.</li>
                    <li>A screenshot showing how many JUnit tests passed.Click on the "Submit" button on this page, then add the following files individually:</li>
                </ol>
            </li>
        </ol>
        <p><i>Note: You are turning in the Eclipse project so that I can easily open it and run it on my computer.&nbsp; You are also turning in the .java file so that I can easily provide feedback to you via Canvas. The screenshot of the JUnit tests passed gives us an idea how you did with the test cases. </i></p>
    </div>
</div>




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

___________

## Rubric

[Rubric](Rubric.md)


___________

_this repository is a subset of the CISC191 exercises. It is derived from the CISC191ProgrammingChallenges 
activity hosted by Professor Allan Schougaard, San Diego Mesa College, and not a direct fork._

_This project is to decompose that repository into git submodules_
