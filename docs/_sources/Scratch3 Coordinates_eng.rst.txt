Tell Me Where To Go - Coordinates And Direction
=================================================

.. include:: blocks.txt

.. include:: icons.txt

.. infonote::

  |intro2|


After getting to know the basics of the environment, it is time to learn about how you can send your sprites to the desired location on the stage. To do that, you need to know how the stage is organized and which commands enable movement.

.. sidebar:: Sprite Coordinates

 |stage|

.. |stage| image:: ../_images/2/fig2_1.png

.. topic:: The Stage
      
 When you open Scratch, the stage is automatically created: a white rectangle 480 dots wide and 360 dots high. The smallest dot that can be displayed on a computer graphics screen is called *Pixel*.

 The Stage is where your stories, games and animations will run. It is stationary, like an aquarium, but its inhabitants - Sprites are always moving and interacting with each other. In order to control the sprites' movements easily, each spot on the stage is assigned an address - *coordinates x and y*, these coordinates represent the distance of that particular spot from the center of the stage. The spot, which is located at the center of the stage has the coordinates х=0 and у=0, or (0,0).

 The coordinates allow us to accurately move our sprites around the stage and position them anywhere we want (x, y). The current position of the sprite can be seen in the active sprite's information. 


.. topic:: Functions of the *Motion* Blocks
 
 All commands, which enable positioning of the sprite in the desired location and control its direction and movement, are located in the group of blocks called *Motion*. In this lesson, you are going to learn more about motion blocks and how to use **reporter blocks**, by looking at examples and doing exercises. Reporter blocks do not correspond to language commands, and they cannot stand independently in a script. The function of a reporter block from the *Motion* group is to store the current coordinates and directions of Sprites.

.. topic:: Motion Reporters

 In this group there are |x_position| and |y_position| blocks, which contain the current information on the position of the sprite (its x and y coordinates), and the |direction| block, which represents the direction of the sprite.

 If you want to see the current coordinates and the direction of the sprite, you need to click on the checkbox next to the desired block. If you click on the checkboxes next to motion reporters, displays with which you can monitor the current coordinates and direction of the sprite will appear on the stage.
 
 .. image:: ../_images/2/fig2_2.png
   :width: 400px   
   :align: center
 
 
.. topic:: Absolute and Relative Motion

 You can send your sprite to a specific spot on the stage in two different ways: with absolute or relative motion.

 **Absolute Motion** is moving to a specific spot - destination, regardless of the current position of the sprite. 

 In Scratch you can send your sprite to a given position (х,у) on the stage, that is to say, you can perform absolute motion by using the following blocks:

 - |goto_xy| - go to position (х,у), 
 - |glide_xy| - glide to the position (х,у), 
 - |set_x| - set coordinate x to the position, 
 - |set_y| - set coordinate y to the position. 

 By using the |goto_xy| block the sprite will move instantly to the given position (х,у).

 Similarly, the target will be reached with the block |glide_xy|, but the move would not be instant; it would last a given number of seconds. The higher the number of given seconds, the longer it will take the sprite to reach its destination.

 Another way to set a destination in absolute motion is to independently set the coordinates x and y, using the blocks |set_x| and |set_y|.

 **Relative Motion** is moving to a location defined by the number of steps the sprite will make from the current position. Of course, you also need to set the direction in which the sprite should move (right, up, etc.).

 Another way to set a destination in relative motion is to independently set the coordinates x and y, by using the |change_x| and |change_y| blocks.

 In Scratch, you can send the sprite to a location defined by the number of steps from its current position, that is to say, you can perform relative motion by using the following blocks:
 
 - |change_x| - move a certain amount of pixels horizontally in relation to the current position, 
 - |change_y| - move a certain amount of pixels vertically in relation to the current position (х,у), 
 - |turn_right| - turn right a certain amount of degrees in relation to the current direction, 
 - |turn_left| - turn left a certain amount of degrees in relation to the current direction, 
 - |move_steps| - move a certain amount of steps in the given direction in relation to the current position.
    

.. sidebar::  Direction Blocks
   :subtitle: |point_direction| and |point_towards|

   There are three ways to set a value in the input field of the first block:

   |direction1|

   (1) to select one of the offered values ​​from the drop-down list, for example (0) up;
   (2) type in a new value, instead of the old, for example 45;
   (3) to rotate the blue arrow indicating the direction in the current Sprite information.

   From the drop-down list you can choose towards which object the Sprite in the other block will be directed.

   |direction2|

.. |direction1| image:: ../_images/2/fig2_3.png

.. |direction2| image:: ../_images/2/fig2_4.png

.. topic:: Direction and Rotation

 In addition to the rotation blocks |turn_right| and |turn_left|, which allow you to change the direction in relation to the current direction of the sprite, in Scratch, there is an option to use blocks that set the direction regardless of the current position of the Sprite. 

 These are |point_direction| and |point_towards| blocks. 

 On the following Figure you can find the main direction values which you can set in the input field of the first block: *up* (North), *right* (East), *down* (South) and *left* (West).

 .. image:: ../_images/2/fig2_5.png
   :width: 250px   
   :align: center

 You can also set other values, for example, value 45 will point the sprite in the direction of the northeast, and 135 to southeast. To point it west, you do not need to use negative numbers. You can type in numbers from 180 to 360 instead.  

 The second block points the sprite towards a mouse-pointer or towards some other sprite in the project. By clicking on the white triangle in the value field, you can open the drop-down list and select towards which object you want to point your sprite. For example, in the project "Dinosaur Walk", which will be analyzed later in this lesson, the cat can be pointed towards the mouse-pointer or towards one of the three dinosaurs, which represent sprites in this project. 
  

|study| Study the following examples
------------------------------------

As we have shown the easy way to make our sprite talk in our "Hello World" project, and then by doing exercises upgraded our project so that the sprite really pronounces the text, we will now show the basic commands which will enable us to move our sprite, and then we will upgrade them through different exercises.

Example 1 - Project "The Walk"
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


|1| Click on the *Motion* blocks, then drag the |move_steps| block to the Script Area and click on it. The cat will move 10 steps to the right. 

|2| Click several times on this block and take the cat to the right edge of the screen. 

Clicking repeatedly on the move block has allowed the action assigned by this block, to be repeated several times. Repeating of a particular action can also be achieved by coding. 

|3| Return the cat to the middle of the screen and click the *Control* blocks. Differently shaped blocks from the ones you were using will appear in the Blocks Palette - C shaped blocks with a "mouth" in which you can insert other blocks. 

|4| Select the block |forever| and drag it to the Scripts Area. Clicking on this block enables all the blocks which are inserted into it to run forever (until you stop the running of the program by clicking on the sign *stop*).

|5| Insert a move block into the "mouth" of the repeat forever block and click on them. The cat will go off-screen again.

There is a way to keep the movement of the sprite inside the borders of the screen. That would be to use the block with the command *if on edge, bounce*. This block is located in *Motion* blocks. 

|6| Stop the running of the blocks by clicking the *stop* sign, and then drag the block |if_edge| to the Scripts Area and insert it into the "mouth" of the repeat forever block, below the move block.  

.. sidebar:: The Project Script

  The following Script is added to the cat sprite.

  |script|

.. |script| image:: ../_images/2/fig2_6.png

By running this changed script, the cat will constantly move from one edge to the other, but when it moves to the left, it will be facing the wrong way. Of course, there is a way to fix this. One is to change the way the sprite is moving in the Sprite Information, and the other is to use one of the rotation blocks.

|7| Drag the block |rotation_style| from the *Motion* blocks and place it above the repeat forever block. Make sure that the *left-right* rotation mode is selected from the drop-down list of this block.

|8| Put the |clicked_flag| block at the top of the Script, and by doing this you have completed the "Walk" project. 

You can now run the project by clicking on the *green flag* and stop it by clicking on the *stop* sign. Save the project and continue exploring. 

.......

In our next project, we will show how you can introduce new sprites and backdrops, and how to guide a sprite by using the mouse-pointer. Therefore, before you move on to this example, watch the tutorials *Add a Sprite* and *Add a Backdrop*.

Example 2 – "The Dinosaur Walk"
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

In the previous example, we used the ``repeat forever`` block to make the cat sprite move continuously between the edges of the screen until we stop the running of the project by clicking the *stop* sign. In this project, we will have four sprites, and each of them will have their own scrip, which will determine their behavior. The cat will follow the mouse-pointer forever, and the remaining three sprites - the dinosaurs, will forever be directed towards the cat. The look of the stage at the beginning of the running of the project is presented in the following Figure.

.. image:: ../_images/2/fig2_7.png
   :width: 490px   
   :align: center

**Creation of the Project**

.. sidebar:: Selecting the Backdrop

  You can add a new backdrop to the project by clicking the icon located on the right, next to the Choose a Sprite icon, which is used for selecting new sprites.

  |new_backdrop|

.. |new_backdrop| image:: ../_images/2/fig2_8.png


|1| Click on the icon for choosing backdrops and choose the *Jurassic* backdrop from the backdrop library.

|2| Choose the sprites *Dinosaur1*, *Dinosaur2* and *Dinosaur3* from the Sprites library.

|3| Place your sprites like they are on the Figure above. Yo need to change the direction of the *Dinosaur2*. The default direction value for all sprites is 90 :sup:`о` (they are looking to the right) and their rotation style is *All Around*. All of these settings can be changed in the Sprite Information part or by using appropriate blocks to form scripts added to a particular sprite. In this project, we will use the first option. 

|4| In the Sprite information window set the rotation style as follows: *Dinosaur1* - *don't rotate*, *Dinosaur2* - *left/right*, *Dinosaur3* - *all around*. 

|5| To all dinosaurs add the same script, which will command them to point towards the cat during the running of the entire project. However, they will behave differently because they don't have the same rotation style in their Sprite information settings.
   
|6| For the cat sprite you need to set the commands, which will enable it to point towards the coordinates of the mouse-pointer, that is, to move across the stage the same way the user moves the mouse. 

The Scrips describing the behavior of the dinosaurs and the cat are presented in the following Figure.

.. image:: ../_images/2/fig2_9.png
   :width: 395px   
   :align: center
 
Run the project and move the mouse across the stage. Note that the dinosaurs are tracking its movements in different ways.

.......

.. sidebar:: Selection of the Keys

  The keyboard key that will run the script is selected by clicking on the white triangle next to the key name (space) and then selecting the desired key from the drop-down list. 

  |fig2_11|

.. |fig2_11| image:: ../_images/2/fig2_10.png

Example 3 – "Linear Motion"
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Study the *Use the Arrow Keys* tutorial, and create a project where the cat is led around the stage with the keyboard. 

|1|	Add the |clicked_key| block to the cat.

|2| Choose the key *Right Arrow*.
 
|3|	Choose the |point_direction| block from the *Motion* blocks and connect it to the previous block.

|4|	Choose the |move_steps| block from the *Motion* blocks and connect it to the previous block.

|5|	Press the right arrow key on your keyboard a few times. What happens?

|6|	Duplicate this script (right-click on the first block, then select *Duplicate*).

|7|	In the new script, replace the right arrow with the left arrow, in the block *point in direction* instead of 90 choose -90.

|8|	Press the left arrow key on your keyboard a few times. What happens?

|9|	Similarly, make two more scripts: to guide the cat 10 steps up by pressing the up arrow key, or 10 steps down by pressing the down arrow key.
 
.. image:: ../_images/2/fig2_11.png
   :width: 480px   
   :align: center

.......

Example 4 – "Motion with a Turn"
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

We are going to create one more project for moving sprites by using a keyboard, but with modified functions of the arrow keys. We will remove the blocks for direction, and we will join the *left arrow* key and *right arrow* key with the commands which rotate the sprite 15 degrees to the left or to the right. Also, we will join the *up arrow* key and the *down arrow* key with the block ``move 10 steps``, i.e. ``go -10 steps``. The corresponding scripts will have the following layout.

.. image:: ../_images/2/fig2_12.png
   :width: 435px   
   :align: center

Run the project and test how you can manage sprite's movement.


|ask| Did you understand?
-------------------------

Question 1
~~~~~~~~~~

.. level:: 1

.. mchoice:: stage1
   :answer_a: 1280 pixels wide and 600 pixels high
   :answer_b: 800 pixels wide and 600 pixels high
   :answer_c: 480 pixels wide and 360 pixels high
   :answer_d: 360 pixels wide and 480 pixels high
   :correct: c
   :feedback_a: 
   :feedback_b: 
   :feedback_c: Correct.
   :feedback_d: 
   
   What are the dimensions of the Stage?
   
Question 2
~~~~~~~~~~

.. level:: 1

.. mchoice:: stage2
   :answer_a: in the upper left corner of the Stage
   :answer_b: in the bottom left corner of the Stage
   :answer_c: in the center of the Stage
   :answer_d: depends on the added backdrop
   :correct: c
   :feedback_a: 
   :feedback_b: 
   :feedback_c: Correct.
   :feedback_d: 
   
   Where is the location of the point with the coordinates (0,0)?
   
   
Question 3
~~~~~~~~~~

.. level:: 1

.. mchoice:: blocks1
   :answer_a: Sensing 
   :answer_b: Motion
   :answer_c: Control
   :answer_d: Looks
   :correct: b
   :feedback_a: 
   :feedback_b: Correct.
   :feedback_c: 
   :feedback_d: 
   
   To which group of blocks do the position, direction, rotation and movement management blocks belong to?
   

Question 4
~~~~~~~~~~

.. level:: 1

.. mchoice:: stage3
   :answer_a: yes
   :answer_b: no
   :correct: b
   :feedback_a:  
   :feedback_b: Correct.
   
    Can the Stage run Motion blocks?

Question 5
~~~~~~~~~~

.. level:: 2

.. mchoice:: absolute_motion
   :multiple_answers:
   :answer_a: 
   :answer_b: 
   :answer_c: 
   :answer_d: 
   :correct: a, d
   :feedback_a: 
   :feedback_b: 
   :feedback_c: 
   :feedback_d: 

   Which blocks enable absolute motion? (Select all correct answers)

   .. image:: ../_images/2/q2_5.png
      :width: 530px   
      :align: center

Question 6
~~~~~~~~~~

.. level:: 2

.. mchoice:: relative_motion
   :multiple_answers:
   :answer_a: 
   :answer_b: 
   :answer_c: 
   :answer_d: 
   :correct: b, d
   :feedback_a: 
   :feedback_b: 
   :feedback_c: 
   :feedback_d: 

   Which blocks enable relative motion? (Select all correct answers)

   .. image:: ../_images/2/q2_6.png
      :width: 530px   
      :align: center

Question 7
~~~~~~~~~~

.. level:: 2

.. mchoice:: reporters
   :multiple_answers:
   :answer_a: 
   :answer_b: 
   :answer_c: 
   :answer_d: 
   :correct: b, c, d
   :feedback_a:  
   :feedback_b: 
   :feedback_c: 
   :feedback_d: 

    Which of the blocks represent motion reporters? (Select all correct answers)

   .. image:: ../_images/2/q2_7.png
      :width: 310px   
      :align: center


Question 8
~~~~~~~~~~

.. level:: 3

.. image:: ../_images/2/q2_8.png
   :width: 400px   
   :align: center

.. mchoice:: compass
   :answer_a: Southeast
   :answer_b: Southwest
   :answer_c: Northeast
   :answer_d: Northwest
   :correct: d
   :feedback_a: There it shows a 135 degrees angle.
   :feedback_b: There it shows a -135 degrees angle.
   :feedback_c: There it shows a 45 degrees angle.
   :feedback_d: Correct.
   
   Which side of the world will the Sprite look at after running the |2_8| block?

.. |2_8| image:: ../_images/2/block2_8.png   

Question 9
~~~~~~~~~~

.. level:: 1

In the following Figure you can see a Stage with five different points.

.. image:: ../_images/2/q2_9.png
   :width: 300px   
   :align: center
      
.. mchoice:: coordinates1
   :answer_a: (-200,-40)
   :answer_b: (-200,40)
   :answer_c: (200,-40)
   :answer_d: (200,40)
   :correct: b
   :feedback_a:  
   :feedback_b: Correct.
   :feedback_c: 
   :feedback_d: 
   
   What are the coordinates of the Point A? 
  
.. mchoice:: coordinates2
   :multiple_answers:
   :answer_a: Point A
   :answer_b: Point B
   :answer_c: Point D
   :answer_d: Point E
   :correct: b, d
   :feedback_a:  
   :feedback_b: 
   :feedback_c: 
   :feedback_d: 

   Which points have a negative *y* coordinate?
   (Select all correct answers)


.. dragndrop:: coordinates_various
   :feedback: Try again
   :match_1: A|||(-200,40)
   :match_2: B|||(-160,-60)
   :match_3: C|||(20,0)
   :match_4: D|||(100,120)
   :match_5: E|||(180,-80)
    
   By dragging the rectangles, pair the points with their coordinates.

Question 10
~~~~~~~~~~~

.. level:: 2

In the following Figure you can see a Stage with six different points.

.. image:: ../_images/2/q2_10.png
   :width: 300px   
   :align: center
      

.. dragndrop:: coordinates_symmetrical
    :feedback: Try again
    :match_1: A|||(-160,80)
    :match_2: B|||(-160,-80)
    :match_3: C|||(160,-80)
    :match_4: D|||(80,0)
    :match_5: E|||(160,80)
    :match_6: F|||(0,80)
    
    By dragging the rectangles, pair the points with their coordinates.


.. mchoice:: symmetry_х
   :answer_a: Point А
   :answer_b: Point В
   :answer_c: Point С
   :answer_d: Point D
   :correct: c
   :feedback_a: This should be the point which has the same x, and the opposite value of the y coordinate as the Point E. 
   :feedback_b: This should be the point which has the same x, and the opposite value of the y coordinate as the Point E.
   :feedback_c: Correct.
   :feedback_d: This should be the point which has the same x, and the opposite value of the y coordinate as the Point E.
   
   Which point is symmetrical to the Point E with respect to the *x* axis?

.. mchoice:: symmetry_у
   :answer_a: Point А
   :answer_b: Point В
   :answer_c: Point С
   :answer_d: Point D
   :correct: a
   :feedback_a: Correct.
   :feedback_b: This should be the point which has the opposite value of the x coordinate, and the same y coordinate as the Point E.
   :feedback_c: This should be the point which has the opposite value of the x coordinate, and the same y coordinate as the Point E.
   :feedback_d: This should be the point which has the opposite value of the x coordinate, and the same y coordinate as the Point E.
   
   Which point is symmetrical to the Point E with respect to the *y* axis?
 
.. mchoice:: symmetry2
   :multiple_answers:
   :answer_a: A and B
   :answer_b: A and C
   :answer_c: A and E
   :answer_d: D and F
   :correct: a, b, c
   :feedback_a: 
   :feedback_b: 
   :feedback_c: 
   :feedback_d: 

   Which points are equidistant from the *y* axis? (Select all correct answers) 

|try| Try it!
-------------

Exercise 1 - Tracking the Position of the Sprite
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. level:: 1

.. infonote::

  |1| Drag the cat Sprite to the upper left corner of the Stage, and then check the Sprite information to see the coordinates of the new position.

  |2| Then drag it to the upper right corner of the Stage and check again the coordinates of the position where you left it.

  |3| Repeat what you have just done by moving your Sprite to the bottom part of the Stage. In which positions on the Stage did the coordinate x have the negative value, and in which did the coordinate y?

  |4| Import the *Apple* Sprite from the Sprite library. A blue frame should appear around the thumbnail of the new Sprite in the Sprite list, which means that the Sprite is active. If not, click on its thumbnail in the Sprite list. 
       
  |5| Check the variables *х position* and *у position* at the bottom of the *Motion* group of blocks. *Apple: x position* and *Apple: y position* monitors will appear on Stage.

  |6| Now drag the *Apple* Sprite to different positions on the Stage and track how its coordinates change by looking at the monitors.

.......

Exercise 2 - Setting the Position of the Sprite by Using the Absolute Motion Blocks
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. level:: 2

.. infonote::

  |1| Click on the Stage picture next to the Sprite list. A blue box will appear around the Stage thumbnail, which means that the Stage is in focus.

  |2| Click on the *Choose a backdrop* icon, and then choose the *Xy-grid* backdrop from the *Backdrop library*.

  |3| Now click on the *Code* tab to get the Block Palette instead of the backdrop list. 

  |4| In the *Motion* blocks you will see a message *Stage selected: no motion blocks*, which is understandable because the Stage, which is now active, cannot move.
  
  |5| Click on the cat sprite in the sprite list. When a blue frame appears around the sprite's thumbnail, the *Motion* blocks will return.

  |6| Drag the |goto_xy| block to the scripts area, and then change the value of x to 120, and the value of y to 100.

  |7| Click on the changed block in the scripts area. What happens?

  |8| Drag the |glide_xy| block to the script area, and then change the value of x to -120, and the value of y to 100. What happens when you click on this block?

  |9| Look where you can find the sprite after clicking the block in which you have previously changed the values for x and y. For example, where will the Sprite be if both coordinates are negative, if they are off-stage, etc? 

........

Exercise 3 - Absolute and Relative Motion
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. level:: 3

.. infonote::

  Try to guide the Sprite from point A to point B by using different *Motion* blocks.
   
  |1| Set *Хy-grid* from the Backdrop library as the backdrop.

  |2| Select two new sprites from the sprite library - letters A and B (Block-A and Block-B).
  
  |3| Set the letter A in the lower-left corner of the Stage in the position (-200, -120), and the letter B in the upper right corner in the position (200, 120). The most precise way to do this is to add the |goto_xy| block to the letter A (drag it to the scripts area while the letter A is active) and enter the appropriate coordinates х and у, and then click on the block. Follow the same steps for the letter B.
  
  |4| Add the |goto| block to the cat, and select *Block-A* from the drop-down list (which will appear when you click on the white triangle in the selection box). **Note**. |goto| |!=| |goto_xy|. 
   
  |5| Click on the |goto| block and the cat will be behind the letter A. 
  
  |6| Click on the |goto_layer| block from the *Looks* group of blocks and the cat will be in front the letter A.
  
  .. image:: ../_images/2/ex2_3.png
     :width: 220px   
     :align: center

  |7| Now in the |goto| block select *Block-B*, and then click on it. The cat will immediately be in front of the letter B. 

  |8| Add the |glide_to| block to the cat, and select *Block-A* from the drop-down list, then click on it. The cat will glide for 1 second to the letter A. **Note**.  |glide_to| |!=| |glide_xy|. 
    
  |9| Try the third way. First, add the |point_towards| block to the cat, and from the drop-down list select the option where the cat points towards the *Block-A* sprite. **Note**.  |point_towards| |!=| |point_direction|

  Click on the |move_steps| block until the cat reaches the letter A.

.......

Exercise 4 - Using the Rotation Style and Direction Blocks
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. level:: 2

.. infonote::

 Create a project in which sprites will behave the same as the sprites in the "Dinosaur Walk" project, but don't make any changes in the Sprite information window. Instead, set the rotation style and the direction with scripts added to the sprites. Save this project under the name "Dinosaur Walk2".

.......

Exercise 5 - Adding New Sprites to Existing Projects 
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. level:: 2

.. infonote::

 Use the "Walk" project for creating a new project where you will introduce a new sprite. This can be a dog or a mouse, which should always point towards the cat. Add the backdrop of your choosing. Add the rotation style to the script determining the behavior of this new sprite. Don't make any changes to the script added to the cat. Save this project under the name "Walk2".

|bug| Debug it!
---------------

Bug 1
~~~~~~~~

The pupil wanted to make a simple animation of the cat’s movement by changing his costume. Therefore, he/she added the following script. 

.. image:: ../_images/2/bug2_1.png
    :width: 220px 
    :align: center

However, nothing happened. What did the pupil do wrong? 

Bug 2
~~~~~~~~

The pupil wanted his sprite to step between the left and the right edge of the Stage. So he/she inserted the *switch costume*, *move 10 steps*, and the *if on edge bounce* blocks into the repeat forever block. However, he/she didn't like the fact that the sprite is facing the wrong way when moving towards the left edge of the stage. What does he/she need to do to correct this?
   
  
|book| Summary
--------------

In this lesson, we showed how we can determine the exact position of a point on the stage by looking at the two coordinates. We can send sprites to a particular position on the stage by using the absolute and the relative motion blocks. Absolute motion is moving the sprite to a new location on the stage - destination, regardless of its previous position. On the other hand, Relative motion is changing the position of the sprite in relation to its previous position on the stage. The stage cannot run motion blocks. By looking at project examples and by doing the exercises, we learned how we can control the movement of our sprites by using our keyboard and our mouse.

**Scratch projects**: 2Studio_

.. _2Studio: https://scratch.mit.edu/studios/25119440/

**New concepts**:  pixel, coordinate system, coordinates, motion blocks, motion reporters, absolute motion, relative motion, direction, rotation mode.

**Scratch commands**: |motion_blocks| - |move_steps|, |turn_right|, |turn_left|, |point_direction|, |point_towards|, |goto_xy|, |goto|,  |glide_xy|, |glide_to|, |set_x|, |set_y|, |change_x|, |change_y|, |if_edge|, |rotation_style|, |x_position|, |y_position|, |direction|; 

|events_blocks| - |clicked_key|; |looks_blocks| - |*| |goto_layer|,  |*| |switch_costume|; |control_blocks| - |*| |forever|.

Note. Blocks marked with the |*| sign will be discussed in the lessons that follow.

|project| Create a projects
---------------------------

Project 1 - "Two Players"
~~~~~~~~~~~~~~~~~~~~~~~~~~~

Start a new project that you will call “Two Players”. Put two sprites on the stage, one on the left and the other on the right. Set the sprites to point at each other. Add scripts which will allow them to move back and forth, and to turn clockwise and counter-clockwise.

The control keys for the first Sprite should be:

•	Up Arrow - The Sprite goes forward in a straight line,

•	Down Arrow - The Sprite goes back in a straight line,

•	Left arrow - The Sprite turns counter-clockwise,

•	Right arrow - The Sprite turns clockwise.

The control keys for the second Sprite should be:

•	Key W - The Sprite goes forward in a straight line,

•	Key S - The Sprite goes back in a straight line,

•	Key A - The Sprite turns counter-clockwise,

•	Key D - The Sprite turns clockwise.
