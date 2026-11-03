# 🎵 Spotify Music Microservice (Backend)

This is the backend server for the **Spotify Vibe Check** app. It runs on **Node.js** and serves song data as JSON over HTTP whenever frontend clients ask for it.

---

## 🚀 How to Deploy on Render

1. Log into [Render](https://render.com) (sign up with your GitHub account).
2. Click **"New +"** ➔ **"Web Service"**.
3. Choose **"Build and deploy from a Git repository"** and select this backend repository.
4. Fill in the settings:
   * **Name**: `my-spotify-music-api` (or any name you like)
   * **Language / Runtime**: `Node`
   * **Branch**: `main`
   * **Build Command**: *(leave empty)*
   * **Start Command**: `npm start` (or `node server.js`)
   * **Instance Type**: `Free`
5. Click **"Deploy Web Service"**.
6. Once deployed, Render will give you a public URL (e.g. `https://my-spotify-music-api.onrender.com`).
7. Copy this URL and paste it into your Vercel frontend website!

---

## 📡 Available API Endpoints

| Endpoint | Method | What It Returns |
| :--- | :--- | :--- |
| `/api/track` | `GET` | Returns a random song object in JSON format |
| `/api/status` | `GET` | Health check verifying that the microservice is online |
| `/` | `GET` | Friendly welcome message and API index |

---

## 🎯 Customization Challenge: Add New Songs on the Server

1. Open `server.js` on GitHub.
2. Click the **Pencil icon** (✏️) to edit.
3. Scroll down to the `const songs = [...]` list and add your own favorite track!
4. Click **"Commit changes"**.
5. Render will automatically redeploy the new songs within seconds!
