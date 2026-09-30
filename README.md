# Agimat Studio · Beta 0.1

A TikTok LIVE helper for streamers: live chat with photos, alerts, goals,
shoutouts, polls, a streamathon clock, your socials, and Meld Studio controls.

This is a **private beta**: you need a beta code from Pepe.

## 1. Download
Open **Releases** (right side of this page) → **v0.1-beta** → download
**AgimatStudio-Beta-0.1.zip**.

## 2. Unzip
Right-click the zip → **Extract All** → choose your **Desktop** (or Documents).
Not Program Files. Open the folder and double-click **AgimatStudio.exe**.

## 3. "Windows protected your PC"
Windows shows this for new apps that aren't signed (signing costs money).
Click **More info** → **Run anyway**. Some antivirus apps complain too,
because Agimat listens for your hotkeys; if yours blocks it, allow
AgimatStudio.exe.

## 4. Paste your code
Copy the whole code Pepe sent you (it starts with `AGIMAT-`), paste it, press
**Start**. The top of the window shows how many days you have left. When it
runs out, ask Pepe for a new code: your settings are kept.

## 5. Connect
Type your TikTok name (no @) and press **Connect Stream** while you're LIVE.

## 6. Put it on stream
Open **http://localhost:8000/monitor.html** in your browser: that's your
Live Monitor. Under **Widgets**, press **📋 Copy link** on the one you want,
then add it to your streaming app:
- **Meld Studio** or **OBS**: add a **Browser Source** with that link.
- **TikTok LIVE Studio**: **Add source → Link** and paste it.

## 7. Scene buttons (Meld Studio or OBS)
In the Live Monitor's **🎬 Streaming app** box, pick the app you stream with.
- **Meld Studio**: in Meld, **Settings → Advanced → WebSocket Server** on.
- **OBS (version 30 or newer)**: in OBS, **Tools → WebSocket Server Settings**
  → tick **Enable WebSocket server** → **Show Connect Info** → copy the
  **Server Password** and paste it in the box.

You get your scene buttons (the live one lights up), mic mute, record, and
the streamathon can switch to your ending scene. TikTok LIVE Studio has no
remote control, so it gets everything except scene buttons.

## 8. Spotify (optional)
You need **Spotify Premium** (Spotify's rule for apps like this, and for
controlling playback).
1. Go to **developer.spotify.com/dashboard**, log in, **Create app**.
2. Any name. Redirect URI, exactly: `http://127.0.0.1:8000/spotify/callback`
   (the numbers, not "localhost"). Tick **Web API**. Save.
3. Open the app's **Settings**: copy the **Client ID** and **Client secret**.
4. In Agimat's **Music Bot** tab, paste both and connect.

Keep your Client secret private, like a password.

## Your files
Settings, media and data are in **Documents\Agimat Studio**. New version:
delete the old AgimatStudio folder and unzip the new one; your settings stay.

## Privacy
Agimat runs on your PC. It talks to TikTok (through the TikTokLive library
and the connection service it uses), and to Spotify, Meld or OBS only if you
connect them. Your OBS password stays on your PC. The widget pages can only
be opened on your own PC.

## Problems or ideas?
Message Pepe with a screenshot.
