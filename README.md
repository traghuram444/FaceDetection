# FaceDetection

Educational full-stack face-detection demo built with React, Express, PostgreSQL, and the Clarifai API.

## Overview

The application accepts an image URL, sends it to a configured Clarifai face-detection model, and renders the returned face bounding boxes in a React interface. It also includes an Express backend with PostgreSQL-backed registration and sign-in flows.

## Architecture

```text
Face_recognition-master/
├── face-recognition/  React client and image-box rendering
└── server/            Express API, PostgreSQL access, and authentication routes
```

## Technologies

- React and JavaScript
- Express and Node.js
- PostgreSQL with Knex
- Clarifai face-detection API
- bcrypt-based password hashing in the backend

## Running locally

The client and server are separate projects inside `Face_recognition-master`. Install dependencies in each project, configure a local PostgreSQL database and a Clarifai API key, then start the server and client using their package scripts.

The repository intentionally leaves external service configuration to the local environment. It is an educational API-integration project, not a trained face-recognition model or a production identity system.

## Limitations

Results depend on the external Clarifai model and API configuration. The application detects face regions; it does not identify people or provide a locally trained computer-vision model.
