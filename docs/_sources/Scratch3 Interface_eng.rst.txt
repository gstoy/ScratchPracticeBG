Scratch Programming Environment
================================

.. include:: blocks.txt

.. include:: icons.txt

.. infonote::

  |intro1|

   
Would you like to create your own computer game, animated story, instruction or presentation? Scratch is a programming language that enables you to create all of these things, and more.

Unlike the majority of common programming languages, Scratch is a *visual* programming language – instead of typing commands by using the keyboard, programs are created by connecting color coded blocks, which represent different commands, something like making different objects by using LEGO bricks.

In Scratch, **projects** are created. The first step in creating a project is adding Sprites that will participate in it. Different looks, sounds and behaviors can be attached to all of the sprites. The behavior of a sprite is described by the **Script**. The project contains one or more scripts; each is associated with a sprite or a stage - the place where the project takes place.

In order to write a program in Scratch, first, it is necessary to get to know the environment in which the programs are created or its **interface**.

.. topic:: Scratch Programming Interface.

 The following Figure shows the interface of the Scratch programming language. 

 .. image:: ../_images/1/fig1_1.png
   :width: 800px   
   :align: center

 First, we will learn about the basic functions of its main parts, and in the following lessons we will get to know other components of the environment.

 **The Stage** is the place where your stories, games and animations will come to life. The stage itself is stationary, but it has sprites on it that can move and interact with one another.

 **The Blocks Palette** is the area where all available commands of the Scratch programming language are kept. It is called “palette” because it looks like a palette a painter uses while painting. However, unlike a painter, a programmer creates live pictures with objects that interact with each other.

 **Scripts Area** is a place where the scripts are created. To make a script, you need to drag blocks from the Blocks Palette to the Scripts Area and snap them together.

 **The Sprite List** displays names and thumbnails of all sprites in your project.

 **The Menu Bar** allows you to set project management commands and adjust the environment itself.

.. topic:: My First Program

 Even the longest journeys begin with a single step. That first step in learning a programming language would be to write a program which would display the words "Hello World" on the screen. This is how we will start mastering Scratch.

 Whenever Scratch is activated, the **stage** is automatically created, and it is composed of a white rectangle with a cat **sprite** in it.

 The stage and sprites are **objects** whose behavior is programmed by Scratch commands. We build **scripts**, which describe the behavior of the objects, by using blocks, which correspond to language commands. Every object has its own behavior, even the stationary stage, which, for example, can change its backdrop.

 Stages and sprites can be associated with **graphics** (pictures - drawings, photos) and **sound** files in addition to scripts. The look of a sprite is called the **costume**, and the look of the stage a **backdrop**.

 **The Sprite list** shows thumbnails of all the sprites involved in the project. The name of each sprite is written below the thumbnail.

 You can view and modify the current sprite information in the window above the Sprite List.

 .. image:: ../_images/1/fig1_2.png
   :width: 650px   
   :align: center
 
 .. infonote::

  1. The *Name* of the sprite can be changed by typing a new name in the sprite's name field.

  2. The *Position* of the sprite on the stage is defined by its coordinates x and y.

  3. Whether the sprite is visible or hidden on the Stage, depends on what is checked in the *Show* checkbox.

  4. The *Size* of the sprite is expressed as a percentage of the original size. The number 100 indicates that the Sprite is viewed in its normal size.

  5. The *Direction* indicates the direction in which the Sprite will move. The white arrow in the blue circle shows the direction of the sprite. You can change the direction by rotating the arrow or typing the appropriate number in the direction field (0: up, 90: right, 180: down, -90: left). |rot_style| indicates the rotation style, which can be: *all around*, *left-right*, or *don't rotate*.

 To create a script, you need to drag the appropriate commands from the command palette to the script area of the active object and link them.

 **An active object** - a sprite or a stage, is recognized by the fact that there is a blue frame around its thumbnail in the Sprite list. Everything we create: scripts that describe behavior, costumes that describe the look, sounds that will be heard when we run our project, is associated with the object that is active in the moment of creation. 

 Scripts are created by snapping blocks together. Clicking anywhere within a series of blocks runs the complete script, which is executed from top to bottom.

|study| Study the following examples
-------------------------------------

Example 1 - The “Hello World” Project 
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

The simplest possible script will be added to the Scratch trademark cat. It consists of a single command - a block that allows the Sprite to say *Hello World*, that is, the text will appear in a speech bubble next to the cat. This is how you do it:

|1| Click on the *Looks* group of blocks located in the Blocks Palette. A group of purple blocks, designed for attributing visual effects to sprites, will appear. 

|2| Drag the |say_sec| block to the script area.

|3| Then, instead of the text *Hello*, type *Hello World* and click on the modified block.

.. image:: ../_images/1/fig1_3.png
   :width: 740px   
   :align: center

The speech bubble with the text *Hello World* will remain on the Stage next to the cat for 2 seconds. As you can see, it is quite simple.

Now we are going to add a few more |say_sec| blocks to make our sprite say a few more sentences. 

We will show here two different ways you can add a block that already exists in the scripts area.

- 1. By repeating the steps we have already done: one more time, drag another |say_sec| block from the Blocks Palette and instead of the text *Hello* type *I am a cat*. 

- 2. Right-click on the block in the Scripts Area to open the shortcut menu and select *Duplicate* from it. Then write the text you want in the copy of the block, in our example - *I like to walk*. This way you can work faster, since you can copy multiple blocks that have been previously linked, with just one move.

.. image:: ../_images/1/fig1_4.png
   :width: 740px   
   :align: center
 
To make the blocks run automatically one after the other, you need to put them together in a stack. We do this by dragging blocks. When the blocks get close to one another, a shadow appears around the block above, which means that the blocks will be connected. When we connect all three blocks in a stack and then double click on them, the Sprite will say all three sentences one after another. 

**Running the Project**

You noticed that the block you used had a notch at the top and a bump on the bottom. A block that has this shape is called a **stack block**. Most of the Scratch commands are assigned to stack blocks. However, the first block, which indicates which event will trigger the script, does not need to have a notch at the top, since there are no blocks above it. These blocks are called **hat blocks** and most of them can be found in the *Events* group. Click on the *Events* group in the Blocks Palette and drag the |clicked_flag| block to the Scripts Area. Then place this block on top of the previously formed stack, and your project is done. To run it click on |g_flag| above the top left corner of the stage.  

**Saving the Project**

This is how you can save the project on your computer:

|1| Click on *File* in the Menu Bar.

|2| Select the option *Save to your computer*.

|3| In the opened dialogue window, select a folder and enter the name under which you will save your project, and then click the *Save* button.

**Upgrading the Project**

Instead of displaying a speech bubble with the text in it, the cat can actually say what is written. You can do this by selecting the |play_until| block from the *Sound* group, and then recording in the sound editor the sentence you want the cat to say. After you have done this, select the recorded speech instead of *meow* from the drop-down list of this block. 

However, in this version of Scratch, you can do more than that. Among the extensions, there is a *Text-to-Speech* group that allows sprites to start speaking for real. You can do this only if you are connected to the Internet because it uses *Amazon Web Services*.


|ask| Did you understand?
-------------------------

Are you confused as to how you can answer the questions which have not been explained in the text yet? Simply open Scratch and try!

Question 1
~~~~~~~~~~

.. level:: 1

.. mchoice:: interface1
   :answer_a: script
   :answer_b: object
   :answer_c: interface
   :answer_d: code
   :correct: c
   :feedback_a:  
   :feedback_b: 
   :feedback_c: True.
   :feedback_d: 
   
   What is the name of all windows and icons, which are visible when you open Scratch?
  

Question 2
~~~~~~~~~~
.. level:: 1

Some parts of the Scratch interface are marked with numbers from 1 to 5. 

.. image:: ../_images/1/q1_2.png
   :width: 600px   
   :align: center
      
.. dragndrop:: interface2
    :feedback: Try again
    :match_1: stage|||4
    :match_2: blocks palette|||2
    :match_3: scripts area|||3
    :match_4: sprite list|||5
    :match_5: menu bar|||1
    
    Drag the name of each part of the environment to the corresponding position in the image.


Question 3
~~~~~~~~~~

.. level:: 1

.. mchoice:: interface3
   :answer_a: yes
   :answer_b: no
   :correct: b
   :feedback_a: False. Project needs to have а stage with at least one backdrop.
   :feedback_b: True.
   
   Can you make a project that doesn't have a stage?

Question 4
~~~~~~~~~~

.. level:: 1

.. mchoice:: interface4
   :answer_a: yes
   :answer_b: no
   :correct: a
   :feedback_a: True.
   :feedback_b: False. The project can have only scripts which are associated with the stage.
   
   Can you make a project that doesn't have sprites?

Question 5
~~~~~~~~~~

.. level:: 1

.. mchoice:: interface5
   :answer_a: yes
   :answer_b: no
   :correct: b
   :feedback_a: False. The object needs to have at least one look, the stage - backdrop, and the sprite - costume.
   :feedback_b: True.
   
    Can you create a stage or a sprite without assigning a look to them?

Question 6
~~~~~~~~~~

.. level:: 1

.. mchoice:: interface6
   :answer_a: yes
   :answer_b: no
   :correct: b
   :feedback_a: False. Some sprites and stages can just be decoration for the project.
   :feedback_b: True.
   
   Does every object in the project need to have at least one script associated with it?

Question 7
~~~~~~~~~~

.. level:: 1

.. mchoice:: interface7
   :answer_a: yes
   :answer_b: no
   :correct: a
   :feedback_a: True. 
   :feedback_b: False. The project starts running when you click on the Green Flag, and it stops when you click on the Red Stop Sign.
   
   Do the Green Flag and the Red Stop Sign allow you to control script execution?

Question 8
~~~~~~~~~~

.. level:: 1

.. mchoice:: interface8
   :answer_a: menu bar
   :answer_b: sprite list
   :answer_c: scripts area
   :answer_d: blocks palette
   :correct: b
   :feedback_a:  
   :feedback_b: True.
   :feedback_c: 
   :feedback_d: 
   
   What is the name of the place where we can find thumbnails of all sprites participating in the project?  

Question 9
~~~~~~~~~~

.. level:: 1

.. mchoice:: interface9
   :answer_a: looks
   :answer_b: suits
   :answer_c: costumes
   :answer_d: masks
   :correct: c
   :feedback_a:  
   :feedback_b: 
   :feedback_c: True.
   :feedback_d: 
   
   The sprite can have one or more _______, this enables it to change its appearance during the running of the project. 

Question 10
~~~~~~~~~~~

.. level:: 1

.. mchoice:: interface10
   :multiple_answers:
   :answer_a: presentations
   :answer_b: scripts
   :answer_c: graphics files
   :answer_d: sound files
   :correct: b,c,d
   :feedback_a:  
   :feedback_b: 
   :feedback_c: 
   :feedback_d: 

   What can be assigned to stages and sprites?
   (Select all correct answers)  



It's time to explore.

|Try| Try it!
-------------

Exercise 1 - Exploring *Tutorials*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. level:: 1

.. infonote::

 By clicking on *Tutorials* in the Menu Bar (1) you will open a library of short instructions for creating different projects in Scratch. Select the tutorial *First Steps* (2) and watch the associated video (3), then by clicking on white arrows in green circles (4) you can review the steps for creating simple projects similar to our "Hello World".

 .. image:: ../_images/1/ex1_1.png
   :width: 1000px   
   :align: center

.......

Exercise 2 - Sprite Information
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. level:: 1

.. infonote::

 |1| In the active sprite's information, change the direction of movement of the sprite so that it goes up. What will happen on the stage?

 |2| How will the sprite be directed if you set a value of 45 degrees as the direction of movement?

 |3| With the mouse-pointer move the sprite and follow what is happening with the coordinates in the active sprite's information.

 |4| Check what happens to the sprite if the option for it to be hidden is selected in the *Show* box. How can you get the sprite back on the stage? 

 |5| Change the name of the active sprite.

.......

.. sidebar:: Choose a Sprite
    
    You can add a new Sprite by clicking on the button located in the bottom right corner of the Sprite List.

    |new_sprite|

.. |new_sprite| image:: ../_images/1/fig1_5.png

Exercise 3 - Introducing New Sprites
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
      
.. level:: 1

.. infonote::
  
 |1| Import a new sprite from the Sprite Library. 

 By clicking on the *Choose a Sprite* button you will open the Sprite Library. Now you need to click on the sprite you like - for example, the ballerina sprite. 

 |2| Draw a new sprite using the built-in image editor. 

 By clicking on the *Paint* option, instead of the *Code* tab you will open the *Costumes* tab. The Paint Editor, which you can use to draw your new sprite, will open where the Script Area was previously. When you are done just click the *Code* tab.
  
 |3| Import a few surprise sprites from the Sprite Library.

 |4| Import a new sprite from a file by clicking the *Upload Sprite* option.

.......

Exercise 4 - Duplicating and Deleting Sprites
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. level:: 1

.. infonote::

 |1| Right-click on the sprite in the Sprite List, choose the option *duplicate* from the shortcut menu and make 3 copies of the sprite.

 |2| Remove one of the copies by choosing *delete* from the shortcut menu.

 |3| Enter numbers 50 and 200 in the *size* boxes so that one copy is half the size and one copy is double the size of the original.

.......

Exercise 5 - Using Sound  
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Warning.** You can complete this exercise only if your computer has an audio recording option! 

Explore the Tutorial *Record sound*, and try to create a project where the sprite will say the phrase "Hello World" in your voice. As this exercise uses the Sound Editor which we will introduce later, you can skip this and come back to it later.

.. level:: 2

.. infonote::

 |1| Open Scratch.

 |2| Click on *Sound* group of commands located in the Blocks Palette. A group of light purple blocks for the sound effects that can be assigned to the sprites will appear.
  
 |3| Drag the |play_until| block to the Scripts Area. 
  
 |4| Click on the *Sound* tab. The Sound Editor window will open.
  
 |5| Click on *Choose a Sound*, then select the recording option.

 |6| When the Recording dialogue box appears, click on the *record* button, then say the phrase "Hello World" and then stop recording.

 |7| Listen to the recording and if you like it click *Save*. Another sound named *recording1* will appear in the list of sounds associated with the cat sprite.

 |8| Go back to the *Code* tab and instead of the sound *meow* choose *recording1*. If you click on the green flag, the cat will say the sentence you recorded.

 |9| Add two more |play_until| blocks, then add to them the recordings of two more sentences you want the cat to say.

 |10| Snap the blocks together to form a stack and place |clicked_flag| block on the top. Save this project under the name "Hello World2".

.......

Exercise 6 - Using the Extension *Text to Speech*  
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Warning.**  You can complete this exercise only if your computer is connected to the Internet! 

Explore the Tutorial *Create Animations that Talk* then try to create a project in which your sprite will say "Hello World" with the |speak| block. This exercise uses commands which will be elaborated later, so you can skip this exercise also, and come back to it after.
 
.. level:: 3

.. infonote::

 |1| Open Scratch.

 |2| Click on the |extensions| icon located on the bottom of the Block Palette. The *Extension* blocks will appear.
  
 |3| From the *Extensions* blocks you need to select |voices_extension|. Three new blocks will appear in the block palette. These blocks will enable the sprite to say the text written in the block input field |speak|, in the language set in the |set_language| block. You can also set the type of voice which will be used: female (soprano or alt) or male (tenor or bass). This is done with the |set_voice| block.   
  
 |4| Drag the |set_language| block to the scripts area. 
  
 |5| Drag the |set_voice| block to the scripts area and choose the voice of the Sprite.
  
 |6| Drag the |speak| block to the scripts area and type in *Hello World* into its input field. 

 |7| Add two more |speak| blocks, then type in the other two sentences spoken by the cat.

 |8| Snap the blocks together to form a stack and place the |clicked_flag| block on the top.

 |9| Save this project under the name "Hello World3".

|bug| Debug it!
---------------

Bug 1
~~~~~

The pupil wanted to make his/her own version of the project "Hello World". In it, the sprite should say one sentence after another: *Hello World*, *My name is Mike*, *I like programming*. He attached the sprite to the following script.

.. image:: ../_images/1/bug1_1.png
     :width: 160px   
     :align: center

But after clicking on the green flag, the Sprite said only *I like programming*. What's the bug?

|book| Summary
--------------

In the first lesson we got to know the main parts of the Scratch programming language interface, and we created, ran and saved our first program - project "Hello World". By doing exercises, we showed how we can make sprites say sentences we recorded ourselves by using the Sound Editor or those uploaded from the Text to Speech extension (only if the computer is connected to the internet). 

**Scratch projects**: 1Studio_

.. _1Studio: https://scratch.mit.edu/studios/25119438/

**New concepts**:  interface, Scratch project, active object, sprites, costumes, stage, backdrop, scripts, blocks.

**Scratch commands**: |events_blocks| - |clicked_flag|; |looks_blocks| - |say_sec|,  |say|; |sound_blocks| - |*| 
|play_until|; |voices_extension| -  |*| |set_language|,  |*| |set_voice|,  |*| |speak|.

Note. Instructions marked with the |*| sign will be discussed in the lessons that follow.

|project| Create a project
---------------------------

Project 1 - "About me"
~~~~~~~~~~~~~~~~~~~~~~~~

Create a project that will tell us something about you. Choose a boy or a girl sprite from the Sprite library and attach a script that will make the sprite say the following three sentences: "My name is ...", "I'm ... years old" and "My school is called ...". Insert your information instead of the dots.

