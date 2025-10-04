# Vue-Training

[日本語](../../README.md) | English

A Vue.js 3 + Firebase + RESAS API application for visualizing prefecture data

## RESAS API

RESAS API service was terminated on March 24, 2025.

Currently, this application depends on RESAS API, so the system is not functional.

Reference: [RESAS API Service Termination Notice](https://opendata.resas-portal.go.jp/docs/api/v1/index.html)

## Setup

1. Clone the repository

   ```bash
   git clone <repository-url>
   cd vue-training
   ```

2. Install dependencies

   ```bash
   pnpm install
   ```

3. Configure environment variables
   Create a `.env` file and set the following variables:

   ```env
   # Firebase configuration
   VUE_APP_FIREBASE_API_KEY=your_firebase_api_key
   VUE_APP_FIREBASE_AUTH_DOMAIN=your_project.firebaseapp.com
   VUE_APP_FIREBASE_PROJECT_ID=your_project_id
   VUE_APP_FIREBASE_STORAGE_BUCKET=your_project.appspot.com
   VUE_APP_FIREBASE_MESSAGING_SENDER_ID=your_sender_id
   VUE_APP_FIREBASE_APP_ID=your_app_id
   VUE_APP_FIREBASE_MEASUREMENT_ID=your_measurement_id

   # RESAS API configuration (Note: Service terminated)
   VUE_APP_RESAS_API_KEY=your_resas_api_key
   ```

4. Start the development server

   ```bash
   pnpm serve
   ```

## Tech Stack

- Vue.js 3
- Vuex
- Firebase
- RESAS API (Terminated)
- Chart.js
- SCSS
- ESLint + Prettier

## Features

- Fetch and display prefecture data
- Select prefectures using checkboxes
- Visualize selected prefecture data (chart display)
