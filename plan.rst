========
Activity
========

Introduction
------------
* Activity is used to draw the User Interface of an app, so that the user 
  can perform any actions(eg. clicking a button) or give a visual feedback
* Can be of two types -> Full Screen -> part of the screen (Fragment Activity)
* Any new activity causes the current activity to be closed. However the 
activity is preserved in a stack
* When you press the backbutton, the current activity is destroyed and the previous activity is given the front seat.

* Two important callbacks -> onCreate and onPause
* onCreate -> setContentView -> to set the layout for an activity


Creating a New Activity
----------------------
* A main activity 
NOTE: Example on creating a new one here

A small discussion on Manifest
============================== 
* Any activity created has to have an entry in the Manifest file (this part is 
taken care automatically by eclipse Create New Activity Wizard)
* IntentFilter-> action (MAIN) -> category(LAUNCHer) -> what it means that 
  the current activity is the main activity and the activity can be launched via  the launcher 

* As a sub activity (i.e called from another activity) -> serves two purposes ->  can specify the exact activity to call (or) type of action to perform 
* It can also be an activity from another application

NOTE: A small example here -> emails 

* startActivityForResult -> the activity is started for the whole purpose of 
returning results -> It overrides onActivityResult 
NOTE: A small example her e

Activity LifeCycle
==================
NOTE: Discuss the lifecycle in detail, also pointing out to an example (something that connects to realworld) . Should mention which functions would be useful and point it out... May be a diagram (a simplied one). If you need be, add another example here

NOTE: Also talk about saving the state -> saveBundleState() -> what it means underlying and how it works. This would lead into a discussion about Process LifeCycle too(keep it short)

Advanced topics
===============

* Fragment Activity -> Intro, Philosophy, Small example, lifecycle, 
  static and dynamic fragments
  
* Loader 
  NOTE:This would involve going a little detail about ContentProviders too

NOTE: Need to check out other topics that can fit in Advanced. 








