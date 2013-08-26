Flying Leap 3D
==============

Live Demo #1: http://jaanga.github.io/gestification/projects/flying-leap-3d/r1/flying-leap-3d.html
Live Demo #2: http://jaanga.github.io/gestification/projects/flying-leap-3d/castle/load-castle.html

Built for Nicolás Berríos of Iquique, Chile

Leap.js + Three.js: a Leaped first person camera controller

###Leap Actions

Hand open over Leap device:
* Supports the following FirstPersonControls parameters: moveLeft, moveRight, moveUp, moveUp, moveForward, moveBackword a
* Supports pitch and yaw via lat and lon parameters
* Making fist reatricts camera movement to lat and lon only
* Supports Freeze toggle via a swipe gesture.

### New Mouse Actions
* The app supports all the standard Three.js First Person Control functions
* The fork supports the following additions:
* Turning the scroll wheel controls the speed of movementSpeed and lookSpeed
* Clicking he scroll wheel toggles Freeze on and off.

###New keyboard Commands
	The following new keyboard commands are added to the fork:
	
	````
	switch ( event.keyCode ) {
	case 33: /*page up*/ this.moveUp = true; break;
	case 34: /*page down*/ this.moveDown = true; break;
	
	case 36: /*home*/ this.lookSpeed = 0; this.lat += 1.0; break;
	case 35: /*end*/ this.lookSpeed = 0; this.lat -= 1.0; break;	

	case 188: /*<rf or ,*/ this.lookSpeed = 0; this.lon -= 0.5; break;
	case 190: /*> or .*/ this.lookSpeed = 0; this.lon += 0.5; break;	
	````

###Copyright and License
Copyright &copy; 2013 Jaanga authors

MIT License

###Change Log

2013-08-26 ~ Theo
* Added castle demo

2013-08-24 ~ Theo
* Folders and filess added
* Updates a forked Three.js FirstPersonControls
* Adds freeze and speed controls via mousewheel
* Adds more keyboard commands
* hand2Go2 HTML/JS file is a test bed.
* Adds Leap interaction with FPController
* Provides for XYZ movement plus pitch, yaw and freeze


