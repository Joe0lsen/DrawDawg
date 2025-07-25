# DrawDawg: Architecture

## Overview
DrawDawg is a React app for artists to create custom sets of reference images, and then view them in timed (or un-timed) practice sessions. The app is designed to be able to use any image on the internet (with a valid URL) as a reference. The collection data are saved in local storage, enabling users to create and own their collections without an account. Users can save their collections of URLs as csv, json, or txt to prevent data loss. The app is designed to be used on a desktop or laptop computer.

## Capabilities

- Create/delete collections (saves to local storage)
- Add/remove URL(s) to/from collections
- Download collections (csv, json, txt)
- Load (fetch) collection images (saves to cache)
- Run a session:
  - Choose collection(s)
  - Choose time interval (optional)
  - Start session
  - Pause session
  - Navigate to next/prev image
  - End session

## Features

[Home Page](#home-page)
[Collection Management](#collection-management)
[Session Player](#session-player)

### Home Page

- Welcome/Purpose
- How To
- Ways To Support
  - Post with #DrawDawg or #DrawDawgApp
  - Turn off ad-blocker (or whitelist page)
  - Ko-fi type stuff
  - Paid accounts may become available in the future

### Collection Management

A place for the user to manage their  collections

The Collection Management page should have:

- A list of all previously created (and saved) collections
- An option to create a new collection
- The ability to add and validate URLs to collections
- An option to upload collections
- An option to download collections

Collections are saved in local storage. The user will be prompted to download their collections to prevent data loss (i.e. if browser data gets cleared).

### Session Player

Before starting a session, user chooses session options.

Choose:

- collection(s)
- time interval (optional)
- number of images (all in chosen collection(s) or defined limit)

After making the above selections, the user can click Start. The Session Player appears and displays the images in random order.

The player will have:

- a pause button, if a time interval was chosen
- an "end" (stop) button to end the session
- next/prev buttons
- a timer in the corner, indicating the remaining time (if applicable)

Possible additions:

- Light mode (will be dark by default)
- Flip image horizontally/vertically
- "Star" image (add to favorites)
