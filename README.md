# App Name

## Authors
* John Whee-Jin Choi

## Due
Monday, October 26 at 11:59 PM

## Description
In Homework 3, we gave you most of the basic logic for a functioning Hangman
game. As well, you built UI around the game. In Project 2, you'll be putting
everything together into a well-designed and fully-functional application.
Note that while many of the required features below have already been implemented
in Homework 3, some requirements have changed or been refined.

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
