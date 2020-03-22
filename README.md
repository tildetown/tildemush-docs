# Tildemush documentation

This documentation serves as a reference for
[tilde.town](https://tilde.town)'s tildemush virtual community, lead
by [vilmibm](https://tilde.town/~vilmibm/). It is intended for users who have an account on
[tilde.town](https://tilde.town).
If you are looking for a testing or developing environment, see
[vilmibm](https://github.com/vilmibm)'s notes [here](https://github.com/vilmibm/tildemush)

# Table of contents

- [What is tildemush?](#what-is-tildemush)
- [Purpose and goals](#purpose-and-goals)
- [Conventions used in this documentation](#conventions-used-in-this-documentation)
- [Requirements](#requirements)
- [Getting started](#getting-started)
    - [Starting tildemush](#starting-tildemush)
        - [To start tildemush](#to-start-tildemush)
    - [Creating a new user account](#creating-a-new-user-account)
        - [To create a new user account](#to-create-a-new-user-account)
    - [Logging in](#logging-in)
        - [To log in](#to-log-in)
    - [Resetting your password](#resetting-your-password)
        - [To reset your password](#to-reset-your-password)
    - [Configuring tildemush](#configuring-tildemush)
        - [To configure tildemush](#to-configure-tildemush)
    - [Exiting from the start menu](#exiting-from-the-start-menu)
        - [To exit from the start menu](#to-exit-from-the-start-menu)
- [MAIN tab](#main-tab)
    - [Accessing the MAIN tab](#accessing-the-main-tab)
        - [To access the MAIN tab](#to-access-the-main-tab)
- [WITCH tab](#witch-tab)
    - [Accessing the WITCH tab](#accessing-the-witch-tab)
        - [To access the WITCH tab](#to-access-the-witch-tab)
    - [WORLDMAP tab](#worldmap-tab)
    - [Accessing the WORLDMAP tab](#accessing-the-worldmap-tab)
        - [To access the WORLDMAP tab](#to-access-the-worldmap-tab)
    - [SETTINGS tab](#settings-tab)
    - [Accessing the SETTINGS tab](#accessing-the-settings-tab)
        - [To access the SETTINGS tab](#to-access-the-settings-tab)
- [QUIT tab](#quit-tab)
- [Using tildemush](#using-tildemush)
    - [Sending a message to all users in your current location](#sending-a-message-to-all-users-in-your-current-location)
        - [To send a message to all users in your current location](#to-send-a-message-to-all-users-in-your-current-location)
    - [Quitting tildemush](#quitting-tildemush)
        - [To quit tildemush](#to-quit-tildemush)
- [Scripting with WITCH](#scripting-with-witch)
- [Extra tips](#extra-tips)
    - [Copying text](#copying-text)
        - [To copy text](#to-copy-text)
    - [Pasting text](#pasting-text)
        - [To paste text](#to-paste-text)
    - [Sharing your WITCH code](#sharing-your-witch-code)
        - [To share your WITCH code](#to-share-your-witch-code)
- [Frequently asked questions](#frequently-asked-questions)

<!-- References and todos

add before 'understanding the interface':
https://github.com/vilmibm/tildemush/issues/158

'using tildemush' todos:
in-game commands: https://github.com/vilmibm/tildemush/blob/master/docs/client.md#in-game-commands
break the following into subsections of 'using tildemush'
/dig create a new room, assigning its ownership to the user
/destroy destroy a created object
/create fabricate a new object
/clone create a copy of an object to transfer to another user
/bless open up an object for scripting
/anchor pins an object to a room. It can only be picked up again by the person who anchored it.
/ignore ignore a player or object's messages
/say audibly chat to your current room. default action for entered text.
/yell be loud; chats to your current room, but other rooms hear indistinct yelling from your room. shortcut is **
/emote use a predefined non-verbal action (potentially at another user) shortcut is !
/whisper send a private message to a nearby user.  shortcut is .
/do free-form "character does x"
/get pick up an item in your current room
/examine get item info for something in your current room or inventory; get info on a user
/look get room info
/drop drop an item
/wear add something to your "is wearing" description
/unwear remove something from your "is wearing" description
/wield carry an item in your hands
/unwield put away an item
/quit end game socket session and quit client

'using witch' todos:
https://github.com/vilmibm/tildemush/issues/157

misc references:
23:28 <vilmibm> m455: re: the conversation in tush: it's a little hard to read but you can get a good idea of what WITCH provides here:
                https://github.com/vilmibm/tildemush/blob/master/server/tmserver/witch_header.hy
23:29 <vilmibm> there are also functioning WITCH examples in the test suite, for example,
                https://github.com/vilmibm/tildemush/blob/master/server/tmserver/tests/game_object_test.py#L160
23:30 <vilmibm> (why a common test game object is a horse named Snoozy is a memory I have since lost)
23:31 <vilmibm> ah there are a bunch of WITCH objects in here! just search the page for "incantation"
                https://github.com/vilmibm/tildemush/blob/master/server/tmserver/tests/async_test.py
-->

# What is tildemush?

tildemush is a text-based, programmatic virtual community on the command line. tildemush aims to
provide an environment for creativity, imagination, and art. Currently, tildemush hosted on
[tilde.town](https://tilde.town).

tildemush may look like a chat room, but it is completely programmable, and includes other elements
such as:

* Locations that can be traversed by users
* User-scripted objects that users can interact with
* User inventory and apparel
* A scripting tab for creating objects
* and many more

# Purpose and goals

TODO for vilmibm

# Conventions used in this documentation

* **Note** - Notes signify additional information
* **Tip** - Tips signify an alternate procedure for completing a step
* **Caution** - Cautions signify that damage or loss of data may occur
* **Example** - Examples provide a visual reference of how a procedure would be performed
* `Inline code` - Inline code signifies package names, filenames, commands, and keyboard keys
* ```Code block - Code blocks signify file contents, or an interface element```
* Section - Heading 1s are referred to as "Sections"
* subsections - Heading 2s, 3s, etc. are referred to as "subsections"

# Requirements

* A [tilde.town](https://tilde.town) account

# Getting started

This section describes conventions, which will help you understand the formatting used in this
document, and the requirements for using tildemush.

This section consists of the following subsections:

- [Starting tildemush](#starting-tildemush)
- [Creating a new user account](#creating-a-new-user-account)
- [Logging in](#loggin-in)
- [Resetting your password](#resetting-your-password)
- [Configuring tildemush](#configuring-tildemush)
- [Exiting from the start menu](#exiting-from-the-start-menu)

## Starting tildemush

Starting tildemush will run the software required to connect to the
tildemush virtual community that exists on
[tilde.town](https://tilde.town).

### To start tildemush

**Caution** - Before continuing, you should know that tildemush's
database may be wiped at any time, because it is still under
development. This means that anything you create, may be deleted at
any time.

1. `ssh` into [tilde.town](https://tilde.town)
2. Run `tmclient`
3. Press the `enter` key

## Creating a new user account

TODO: Significance to user

### To create a new user account

TODO: procedures

## Logging in

TODO: Significance to user

### To log in

TODO: procedures

## Resetting your password

TODO: Significance to user

### To reset your password

TODO: procedures

## Configuring tildemush

TODO: Significance to user

### To configure tildemush

TODO: procedures

## Exiting from the start menu

TODO: Significance to user

### To exit from the start menu

TODO: procedures

# MAIN tab

The main tab consists of:

* The chat box, which contains:
  * User messages
  * Events
  * Actions from users
  * Actions from objects
  * Responses from objects

* The location box, which contains:
  * Your current location's name
  * Your current location's description
  * Your current location's user-created objects

* The map box, which contains:
  * TODO: Verify if these are the places you have visited or all places that connect to the current location

* The inventory box, which contains:
  * Number of objects you have
  * Names of objects you have

## Accessing the MAIN tab

The MAIN tab can be accessed from any of the tabs.

### To access the MAIN tab

1. Press `F1`

# WITCH tab

The WITCH tab consists of:

* The object pane, which displays the name and permissions of the object that is being edited.
* The object-scripting pane, which displays the scripts of the object that is being edited. This is the area you will edit the functionality of an object.

## Accessing the WITCH tab

The WITCH tab provides an interface for creating objects.

### To access the WITCH tab

1. Press `F2`

## WORLDMAP tab

The WORLDMAP tab consists of:

* Area blocks, which are user-created locations you can travel to in the MAIN tab.
* Direction names, which are user-created names that a user can type to travel to different area
  blocks in the MAIN tab

## Accessing the WORLDMAP tab

The WORLDMAP tab provides visuals on how all locations are connected.

### To access the WORLDMAP tab

1. Press `F3`

## SETTINGS tab

The SETTINGS tab is under development.

## Accessing the SETTINGS tab

The SETTINGS tab is under development.

### To access the SETTINGS tab

1. Press `F4`

# QUIT tab

The QUIT tab does not contain elements. It serves as a reminder of how
to quit tildemush. See the [Quitting tildemush](#quitting-tildemush) subsection.

# Using tildemush

This section will teach you how to use tildemush and assumes you are familiar with
[tildemush's interface](#understanding-the-interface).

This section consists of the following subsections:

TODO

## Sending a message to all users in your current location

The MAIN tab allows you to interact with users and objects. The MAIN tab is where you will communicate with other users.

### To send a message to all users in your current location

1. Ensure you are in the MAIN tab
2. Type your message
3. Press `Enter`

**Tip**: You can also use the `/say` command to send a message to all users in your current
location.

**Example**:

```
/say hey there! can anyone hear me?
```

## Quitting tildemush

Quitting tildemush will bring you back to your normal shell session on tilde.town.

### To quit tildemush

1. Press `F9`

# Scripting with WITCH

TODO: Explain significance to user

This section consists of the following subsections:

TODO

# Extra tips

This section will describe useful actions for working in tildemush and the terminal.

This section consists of:

* Copying text
* Pasting text

## Copying text

There are various ways to highlight text in the terminal, one of the easiest ways is to use your mouse.

### To copy text

1. Highlight the text you want to copy using your mouse
2. Hold the `Shift` and `Ctrl` keys
3. Press `c`
4. Release the `Shift` and `Ctrl` keys

## Pasting text

[TODO]

### To paste text

1. Hold the `Shift` and `Ctrl` keys
2. Press `v`
3. Release the `Shift` and `Ctrl` keys

**Tip** - Your terminal emulator may allow you to paste text using one of the following methods:

* middle-clicking
* right-clicking, and then selecting `Paste`.

## Sharing your WITCH code

TODO: Significance to user

### To share your WITCH code

TODO: procedures

# Frequently asked questions

TODO

* **Is tildemush the same as IRC?**
  * TODO: *Answer*
