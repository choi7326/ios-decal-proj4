# App Name

## Authors
* John Whee-Jin Choi

## Purpose
[App Name] is a social networking app that allows users to have an avatar 
(circular emoji face which may be customizable later) that responds to texts 
and/or emoji's recieved by another person. 

## Features
* Users can add friends
* Users can send and view messages/gifs/photos/emoji's to each other
* Avatars will react to messages and/or emoji's recieved with simple logic or 
if time permits a smarter ML algorithm
* Extra Feature: allow hand-written messages to be sent to each other like 
the Apple Watch

## Control Flowg
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

### Controller
* LoginViewController
* FriendListTableViewController
* TabBarController
* NotificationListTableViewController
* UserSettingsTableViewController
