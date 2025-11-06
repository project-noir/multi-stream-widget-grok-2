# Multi-Stream Rotating Alerts

Elegant rotating widget for **Twitch + Kick + YouTube** latest followers/subs. Cycles every 7s.

## Quick Deploy to Render (Free)
1. Fork/clone this repo.
2. Go to [render.com](https://render.com) > New > Web Service > Connect GitHub repo.
3. Set Environment: Node > Build: `npm install` > Start: `node server.js`.
4. Add Env Vars (from `.env.example`): TWITCH_CLIENT_ID, etc. (get from platform dev consoles).
5. Deploy! Your URL: `https://your-app.onrender.com/alert.html`

## OBS Setup
- Add Browser Source: URL = your Render URL + `/alert.html`
- Size: 800x200, position on overlay.

## API Setup
- **Twitch**: [dev.twitch.tv/console](https://dev.twitch.tv/console) > New App > Get IDs. Run server to auto-subscribe.
- **Kick**: [kick.com/settings/developer](https://kick.com/settings/developer) > Enable webhooks, point to `/webhook/kick`.
- **YouTube**: [console.cloud.google.com](https://console.cloud.google.com) > Enable YouTube Data API > Get key & liveChatId from stream.

Test: Trigger follows/subs → Watch it rotate! 🎮
