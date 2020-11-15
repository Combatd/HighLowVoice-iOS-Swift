# HighLowVoice-iOS-Swift
iOS App programmed in Swift that records the voice conversation of two people and changes the pitch to high or low

## Learning Goals
* Learn Swift 5, Apple's Programming language, as well as XCode, the Integrated Development Environment used to create native Apple applications for iOS devices.

* Utilize Storyboards to design an interface, and use AutoLayout, UIButtons, and UILabels to create an interface.

* Make a ViewController to react to touch events and change the views according to a user's input.

* Implement AVAudioRecorder, Delegation, and Programmatic Segues in order to set up Audio Recording on an iOS application.

* Setup audio playback with rate, pitch, echo, and reverb. Learn about UIStackViews and class extensions.

* Complete an entire iOS application from start to finish using the Model-View-Controller (MVC) Software Architecture, which allows for separation of concerns and division of responsibilities on a project.

## Phase 1: XCode Storyboard
To start this application, we want to get our Controllers (Application Logic) and Views (User Interface) prototype working before we work with any Model data. 
* Controllers: ViewController - handle touch events, user interaction from Views
* Views: View - can use built-in components from XCode (Autolayout)
    * UIView
    * UILabel
    * UIButton

The ```Main.storyboard``` is where I will design and setup the entire user interface.
Right now, there is only one interface - ViewController. This is the initial ViewController
that loads upon starting the application.

On the ```Main.storyboard```, I want to ensure that the ```Record``` UIButton is always responsive to the screen size of the user's device, whether on an iPhone or iPad. I will add two Constraints, ```CenterX``` and ```CenterY```, to scale the X and Y coordinate values of ```Record``` UIButton on the ```Safe Area``` Canvas.

After testing the Screen Responsiveness in the XCode iOS Simulator, now we need to make sure the button can call upon a function upon being pressed. 
I created an ```@IBAction``` of ```func recordAudio```, then added a "button pressed" message printing to the console to ensure that the
function was successfully called upon a button pressed state (successful debugging!). 


### License Information

```
    HighLowVoice-iOS-Swift: iOS App programmed in Swift that records the voice conversation of two people and changes the pitch to high or low
    Copyright (C) 2020 Mark Calvelo

    This program is free software; you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation; either version 2 of the License, or
    (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License along
    with this program; if not, write to the Free Software Foundation, Inc.,
    51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
```