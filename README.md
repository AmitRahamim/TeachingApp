# TeachingApp
# Online Coding Platform

This project is an online coding web application designed to support real-time collaboration between a mentor (a professional JS lecturer) and students. It enables the mentor to share coding challenges with students, track their progress in real time, and provide immediate feedback through a built-in chat system. A special feature is that once a student's code matches the pre-defined solution, a big smiley face is displayed on the screen.

## Table of Contents

- [Features](#features)
- [Technology Stack](#technology-stack)
- [Installation and Setup](#installation-and-setup)
- [Running the Application](#running-the-application)
- [Project Structure](#project-structure)
- [Usage](#usage)
- [Explanation of Key Files](#explanation-of-key-files)
- [Future Enhancements](#future-enhancements)

## Features

- **Lobby Page:**  
  - Displays a list of coding challenges (code blocks) fetched from MongoDB.
  - Users can select a challenge to work on.

- **Code Block Page:**  
  - Provides a CodeMirror code editor with syntax highlighting.
  - Real-time code updates via Socket.IO enable collaboration.
  - Role-based functionality: the first user becomes the "Mentor" (read-only editor), and subsequent users are assigned "Student" roles (editable editor).
  - A “solution” check: if a student's code exactly matches the pre-defined solution, a large, centered smiley face is displayed.
  - Integrated real-time chat panel with friendly names ("Mentor", "Student 1", "Student 2", etc.).

## Technology Stack

- **Front End:**  
  - React with functional components and hooks.
  - React Router (v6) for client-side routing.
  - CodeMirror for the code editor.
  - Socket.IO client for real-time communication.
  
- **Back End:**  
  - Node.js with Express.
  - Socket.IO for real-time events.
  - MongoDB with Mongoose for data storage.

