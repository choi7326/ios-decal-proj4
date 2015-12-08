# Show

## Authors
* John Whee-Jin Choi

## Current Design:

## Purpose
Show is a simple chat app using the Multipeer Connectivity(MPC) framework 
that allows users to chatwith nearby devices connected to WiFi. As users chat, 
an emoji is tagged with the message, that reflects the emotions of the message. 
NOTE: used a MPC framework tutorial online to help finish this project:
http://www.appcoda.com/chat-app-swift-tutorial/

## Features
* User can send and view messages to each other
* Messages are tagged with an emoji that reflects the emotion of the message
with simple logic

## Control Flow
* NOTE: need 2 devices to properly run this app (one can be the iOS simulator)
* Users are initially presented with a launch screen with the app name shown
* Once the actual app loads, the user is presented with a table view that shows
nearby devices that are visible.
* There is a button on the bottom left that allows users to toggle their visibility
to other devices
* Once the user taps the cell with a visible device name, it sends a request to chat 
with the other device which the other user may accept or decline.
* Once the other user has accepted, both users will transition to another table view
that shows the messages and a text field to enter a message. The messages will be 
tagged with an emotion (5 emotions for now: happy, sad, laughing, neutral, confused)
* There is a X button at the top left of the view to exit the chat

## Control Flow Images

### Load Screen
![alt tag](https://raw.github.com/choi7326/ios-decal-proj4/master/screenshots/LoadScreen.png)

### Toggle Visibility
![alt tag](https://raw.github.com/choi7326/ios-decal-proj4/master/screenshots/ChangeVisibility1.png) ![alt tag](https://raw.github.com/choi7326/ios-decal-proj4/master/screenshots/ChangeVisibility2.png)

### Accept Chat
![alt tag](https://raw.github.com/choi7326/ios-decal-proj4/master/screenshots/AcceptChat.png)

### Chat Screen
![alt tag](https://raw.github.com/choi7326/ios-decal-proj4/master/screenshots/ChatScreen.png)

### End Chat
![alt tag](https://raw.github.com/choi7326/ios-decal-proj4/master/screenshots/EndChat.png)

## Implementation
### Model
* MPCManager.swift - responsible for managing communication between the two devices 

### View
* View - initial view with a UITableView listing the visible nearby devices
* ChatView - UITableView listing showing the messages and a text field to enter
a message

### Controller
* ViewController.swift - controller for View
* ChatViewController.swift - controller for ChatView

## Troubleshooting:
### Cannot open app - Reason: Untrusted Developer 
* Go to: Settings -> General -> Profile -> select developer -> tap Trust "Developer Email"

### App Froze
* Restart app

### Cannot see nearby devices
* Toggle the visibility of your device

## Previous Design: (could not get a working version - overly ambitious)

## Purpose
Show is a social networking app that allows users to have an avatar 
(circular emoji face which may be customizable later) that reflects 
(by changing facial expressions) the emotions of the text message sent 
by the user. The avatar is viewable by the opposite party.

## Features
* Users can add friends
* Users can send and view messages to each other
* Avatars will react to messages and/or emoji's sent with simple logic or 
if time permits a smarter ML algorithm
* Extra Feature: allow hand-written messages to be sent to each other like 
the Apple Watch

## Control Flow
* Users are initially presented with a log-in view
* Once logged in users are logged in there is a tab were users can navigate 
between different views. For now the current views show a list of friends, 
notifications, and settings

## Implementation
NOTE: Will add more implementation details as project progresses.
### Model
* User.swift
* Message.swift
* Avatar.swift
* Notification.swift

### View
* LoginView
* FriendListTableView
* TabBar
* NotificationListTableView
* UserSettingsTableView
* SendMessageView

### Controller
* LoginViewController
* FriendListTableViewController
* TabBarController
* NotificationListTableViewController
* UserSettingsTableViewController
* SendMessageViewController
