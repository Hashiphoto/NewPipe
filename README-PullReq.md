#NewPipe Notifications in MediaStyle
##Description
I updated the background player's notification style to the modern Android mediaStyle. This allows the Android OS to pull data from the image and display it as the background on the lock screen. This is my solution to Feature Request #1570.

I have carefully read the contribution guidelines and adhered to them. I followed the programming style existing in the code, did not add any non-free software, and I made the changes on a feature branch called controls-on-lockscreen. I have tested the application on Android 8.0.0 and above, both emulator and physical device. All the notification buttons work as they did previously. I will maintain this feature if it gets merged with the main project, and I will respond to all change requests and issues with my pull request.

##Limitations
The minimum Android API version for the application has been increased to 27. This is necessary to access MediaStyle, but may prevent users with older operating systems from using the application. The original buttons in the notification are still there - Play, Pause, Stop, Prev/Rewind, and Skip/FForward. Clicking on the notification still opens the NewPipe main application to the Background Player's queue. However, MediaStyle does not allow a progress bar to be displayed in the notification from what I can tell. The styling has not been implemented for the foreground player yet, which should be done before a formal pull request. This was outside the scope of the project.

Even so, I think that this update goes a long way for maintaining a modern look for the application. It also conforms to the current Android style and appears less homebrewed to the average user, making the app more accessible. 

##Testing the Feature
Start playing any video in the background. Everything should function exactly as it did before.