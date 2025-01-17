﻿# website-project

A simple implementation of a social media website in Express.js.

## Features
- Users can register/login/logout with username and password
  - Maximum username length is 20
  - Login session saved until user logs out
  - Passwords are hashed
  - Includes API to directly access user token
    - Can be used to create/edit/delete or like/unlike posts
- Can view all posts from main page
- Can view a single user's posts from that user's page
  - Can navigate to a user's page by clicking on their name in a post
  - Can navigate to own page by clicking on name in navigation bar while logged in
- Post viewing is paginated in pages of 10 posts each
- Can sort posts by most recent or most liked
- Users can create, edit, and delete posts of up to 300 characters
  - Cannot be done from home page, must be done from own page
- Registered users can like posts. Likes are tracked individually for each user

## Usage
- Setup:
    - Requires Node.js installed
    - After unzipping or cloning, run `npm install` from the project directory to install required packages
    - Set up the database according to the included `schema.sql` file, and set the values in `data.js`
- Running:
  - Begin running the website with `node server.js` from the project directory
