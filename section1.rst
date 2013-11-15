Introduction
------------

If you are a website designer, you would know that any website has two 
components , Frontend and Backend and you need to develop them seperately. 
Consider a similar analogy in App development in Android, an Activity forms your
 Presentation layer. It takes care of drawing the User Interface of an app, thus
 giving a visual feedback to the user , also enabling the user to perform any 
action (like clicking a button) .Also, just a website has multiple web pages, 
an android app would also contain one or more activities. So, needless to say, 
whenever you start developing your application, you should start by deciding on the different Activities a particular application will have. 

A sample activity
-----------------

Let us understand how an activity works, by creating a sample application.
Bowing to the programming gods, I would like to start off with "Hello World" app.::
    
      code from helloworld/HelloWorld.java


Well, that was easy was it not. Let me explain.     

* class HelloWorld extends Activity class , which contains methods to create an activity
* We are overriding the method onCreate() from the Activity class. As the name suggests this method is called whenever an activity is created. 
* TextView class creates the text box through which we will display our text.
* setContentView sets the layout for our activity. Here in this example, we have
 only one view., TextView 


But where is our main??
~~~~~~~~~~~~~~~~~~~~~~~
Yes, I can read your mind. Android allows us to specify meta information about an app using a MANIFEST file. Here is ours::

    link to AndroidManifest.xml


Any android activity has to be registered in the manifest file. We can do this by <activity> tag (as seen in our manifest file). It also contains some more details about what intent the activity servers. The <intent-filter> tag serves that purpose . It usually has two sub tags namely <action> and <category>. <action>
specifies that our activity is the MAIN activity and category specifies that
our activity has to be displayed in the Android Launcher(along with other apps)


 











If you have created this activity through eclipse Create New Activity wizard, most of the code is written for you.

     










