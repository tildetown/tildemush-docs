# tildemush handbook

This handbook will serve as a reference for
[tilde.town](https://tilde.town)'s tildemush virtual community, lead
by [vilmibm](https://tilde.town/~vilmibm/). It is intended for new and
experienced users who have an account on
[tilde.town](https://tilde.town). This handbook will provide an
introduction to tildemush, understanding the interface, using
tildemush, and the WITCH scripting language.

<!-- markdown-toc start - Don't edit this section. Run M-x markdown-toc-refresh-toc -->
**Table of Contents**

- [tildemush handbook](#tildemush-handbook)
- [What is tildemush?](#what-is-tildemush)
    - [Describing tildemush](#describing-tildemush)
    - [Creating tildemush](#creating-tildemush)
- [Getting started](#getting-started)
    - [Conventions used in this handbook](#conventions-used-in-this-handbook)
    - [Requirements](#requirements)
        - [Platforms](#platforms)
        - [Software](#software)
    - [Starting tildemush](#starting-tildemush)
        - [To start tildemush](#to-start-tildemush)
- [Understanding the interface](#understanding-the-interface)
- [Using tildemush](#using-tildemush)
- [Scripting with WITCH](#scripting-with-witch)
- [More information](#more-information)

<!-- markdown-toc end -->

<!-- Note to self:
Everytime the TOC is generated, change the "Table of Contents" to an
H1, and remove the title of the document"
-->

<!-- References
23:28 <vilmibm> m455: re: the conversation in tush: it's a little hard to read but you can get a good idea of what WITCH provides here:
                https://github.com/vilmibm/tildemush/blob/master/server/tmserver/witch_header.hy
23:29 <vilmibm> there are also functioning WITCH examples in the test suite, for example,
                https://github.com/vilmibm/tildemush/blob/master/server/tmserver/tests/game_object_test.py#L160
23:30 <vilmibm> (why a common test game object is a horse named Snoozy is a memory I have since lost)
23:31 <vilmibm> ah there are a bunch of WITCH objects in here! just search the page for "incantation"
                https://github.com/vilmibm/tildemush/blob/master/server/tmserver/tests/async_test.py
-->

# What is tildemush?

This section consists of the following topics:

- [Describing tildemush](#describing-tildemush)
- [Creating tildemush](#creating-tildemush)

## Describing tildemush

tildemush is a command line-, text-based virtual community used for
chatting, creating, roleplaying, games, or anything a user can think
of. Currently, tildemush hosted on [tilde.town](https://tilde.town).

tildemush looks like a chatroom with elements such as:

* Your location name
* A list user-created objects that exist in your location
* Your inventory

tildemush also has its own scripting language called WITCH. This
language is used to create in-game objects, which users can interact
with. tildemush provides a separate tab for scripting in WITCH.

## Creating tildemush

[For vilmibm, if they are comfortable with filling this out. Go all out!]

# Getting started

This section consists of the following topics:

- [Conventions used in this handbook](#conventions-used-in-this-handbook)
- [Requirements](#requirements)
    - [Platforms](#platforms)
    - [Software](#software)
- [Quick start](#quick-start)
- [Starting tildemush](#starting-tildemush)

## Conventions used in this handbook

* **Note ++** - Notes signify additional information
* **Tip >>** - Tips signify an alternate procedure for completing a step
* **Caution !!** - Cautions signify that damage or loss of data may occur
* **Example** - Examples provide a visual reference of how a procedure would be performed
* `Inline code` - Inline code signifies package names, filenames, commands, and keyboard keys
* ```Code block - Code blocks signify file contents, or an interface element```
* Section - Heading 1s are referred to as "Sections"
* Topics - Heading 2s, 3s, etc. are referred to as "Topics"

## Requirements

* A [tilde.town](https://tilde.town) account

## Starting tildemush

Starting tildemush will run the software required to connect to the
tildemush virtual community that exists on
[tilde.town](https://tilde.town).

### To start tildemush

**Caution !!** - Before continuing, you should know that tildemush's
database may be wiped at any time, because it is still under
development. This means that anything you create, may be deleted at
any time.

1. `ssh` into [tilde.town](https://tilde.town)

2. Run `tmclient`

3. Use the `up-arrow`, `down-arrow`, and `enter-key` to login or
   create an account

# Understanding the interface

<!-- messy notes for this section begin here
tildemush runs on the command line and contains the following
tabs:

* MAIN
* WITCH
* WORLDMAP
* SETTINGS
* Chatroom
*
with usernames, but it also has different areas users can exist
in. Each area contains users and objects.
-->

# Using tildemush

# Scripting with WITCH

# More information
