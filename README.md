# Swift-Memento-Design-Pattern
An Xcode 9 project, written in Swift 4, demonstrating how to implement the memento design pattern.

In this repo and [accompanying tutorial](), I explain the memento design pattern, meant to capture, represent, and store the internal state of an instance at a specific point in time and then allow you to find that instance's state representation at a later time and restore it. When you restore the state of an instance, it should exactly reflect it's state at the time of capture. While this may sound obvious, you should ensure that all instance property access levels should be respected during capture and restoration, e.g., `public` data should be restored to `public` properties and `private` data should be restored to `private` properties.

Here's the app -- resulting from building this project in Xcode -- in action:

![alt text][logo1]

[logo1]: http://iosbrain.com/wp-content/uploads/2018/08/MementoDemoApp.gif "Memento"

## Xcode 9 project settings
**To get this project running on the Simulator or a physical device (iPhone, iPad)**, go to the following locations in Xcode and make the suggested changes:

1. Project Navigator -> [Project Name] -> Targets List -> TARGETS -> [Target Name] -> General -> Signing
- [ ] Tick the "Automatically manage signing" box
- [ ] Select a valid name from the "Team" dropdown
  
2. Project Navigator -> [Project Name] -> Targets List -> TARGETS -> [Target Name] -> General -> Identity
- [ ] Change the "com.yourDomainNameHere" portion of the value in the "Bundle Identifier" text field to your real reverse domain name (i.e., "com.yourRealDomainName.Project-Name").
