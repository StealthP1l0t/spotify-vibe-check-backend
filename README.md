# 🎵 Spotify Music Microservice (Backend)

This is the backend server for the **Spotify Vibe Check** app. It runs on **Node.js** and serves song data as JSON over HTTP whenever frontend clients ask for it.

---

## 🚀 How to Deploy on Render

1. Log into [Render](https://render.com) using your GitHub account.
2. On your Render dashboard, click **"Deploy a Web Service ➔"** (or click **"+ New"** in the top-right ➔ **"Web Service"**).
3. Under **"Git Provider"**, find and click your backend repository (e.g. `spotify-vibe-check-backend`).
4. On the **New Web Service** configuration screen:
   * **Name**: ⚠️ **Important:** Change this to a unique name with your name in it (e.g., `spotify-backend-alex` or `music-api-sarah`). *This determines your public API URL!*
   * **Language**: `Node` *(autofilled)*
   * **Branch**: `main` *(autofilled)*
   * **Start Command**: `node server.js` *(autofilled)*
   * **Compute**: Scroll down and select the **`$0 / month Free`** tier.
5. Click the white **"Deploy web service"** button at the bottom-left.
6. Once deployed (~1-2 minutes), Render will give you your unique public URL at the top (e.g. `https://spotify-backend-alex.onrender.com`).
7. Copy this URL and paste it into your live Vercel frontend website!

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
