RoundTransparentWindow

This sample code shows how to use Cocoa to create custom-shaped windows and/or transparent window content. It also shows how to change the shape of the window on the fly, and instructs the system to recalculate the drop shadow around the custom window shape. 

Build Requirements
Mac OS X 10.5, Xcode 3.1

Runtime Requirements
Mac OS X 10.5

Packaging List
main.m
Template main method.

Controller
The Controller class implements the -changeTransparency: action, called when the slider on the window is moved.

CustomWindow
Subclass of NSWindow with a custom shape and transparency. Since the window will not have a title bar, -mouseDown: and -mouseDragged: are overriden so the window can be moved by dragging its content area.

CustomView
Subclass of NSView which handles the drawing of the window content. Circle and pentagon graphics are used, switching between the two depending upon the window's level of transparency.

Changes from Previous Versions

1.2 Updated for Xcode Tools version 3.1 and Objective C 2.0.
1.1 Added override of -canBecomeKeyWindow so that controls in the window are enabled.
1.0 Initial version published.
