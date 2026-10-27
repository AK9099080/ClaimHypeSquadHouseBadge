# Discord HypeSquad Badge Script (Updated October 2026) (INSTANT!)

**Current Status (as of October 27, 2026):**  
Discord officially **removed the HypeSquad section** from settings in September 2025, meaning you can no longer join via the in-app quiz. Existing badges remain visible on profiles, but new users can't join officially.

**Good news:** The internal API endpoint (`/hypesquad/online`) **still works**! This console script lets you add a HypeSquad house badge directly.

**Important Warnings:**
- This is **unofficial** and may violate Discord's Terms of Service (considered automation).
- Use at your own risk—account bans are rare for this but possible.
- Works only on the **web version** of Discord (discord.com/app or discord.com/login).
- Your auth token is fetched locally and never leaves your browser.
- Badge appears after refresh; you can only have one house at a time.

## How It Works
1. Fetches your Discord auth token locally (safely).
2. Sends a request to Discord's API to assign you to a house.
3. Badge shows up on your profile instantly (refresh to see).

## Requirements
- Browser (Chrome/Firefox recommended).
- Logged into Discord website app or desktop app if you have console set up on there: [discord.com/app](https://discord.com/app).

## Usage Instructions
1. Open Discord in your browser.
2. Open Developer Console:
   - `Ctrl + Shift + J` (Windows/Linux) or `Cmd + Option + J` (Mac).
   - Or right-click > Inspect > Console tab.
3. Change the `house_id` variable to your preferred `1, 2, 3` house.

Bravery: 1

Brilliance: 2

Balance: 3

5. Paste the entire script and press Enter.

```javascript
let wreq = webpackChunkdiscord_app.push([[Symbol()],{},r=>r]);
webpackChunkdiscord_app.pop();
const chunks = Object.entries(wreq.m)
const findChunkByCode = (...codes) => {
    for (let i = 0; i < chunks.length; i++) {
        const [id,func] = chunks[i]
        const chunkCode = func.toString()

        if (codes.every(code=>chunkCode.includes(code))) return wreq(id)
    }
}

const api = Object.values(findChunkByCode("HTTPUtils")).find(e=>e?.get)

api.post({url: "/hypesquad/online",body:{house_id: 1}})
```
5. Success? Refresh Discord and check your profile badges! 🛡️

To Remove the Badge (Leave HypeSquad)
Run this separate script in the console:

```javascript
let wreq = webpackChunkdiscord_app.push([[Symbol()],{},r=>r]);
webpackChunkdiscord_app.pop();
const chunks = Object.entries(wreq.m)
const findChunkByCode = (...codes) => {
    for (let i = 0; i < chunks.length; i++) {
        const [id,func] = chunks[i]
        const chunkCode = func.toString()

        if (codes.every(code=>chunkCode.includes(code))) return wreq(id)
    }
}

const api = Object.values(findChunkByCode("HTTPUtils")).find(e=>e?.get)

api.del({url: "/hypesquad/online"})
```

# Troubleshooting

Token not found: Fully reload Discord (Ctrl + F5) and try again.
Error 400/403: You might already be in a house—run the remove script first.
Nothing happens: Discord may have updated internals. Search for updated scripts.
Badge not visible? Hard refresh or log out/in.

# Disclaimer
For educational purposes only. Not affiliated with Discord. Use responsibly!

# License
MIT License – Free to use, modify, and share but you have to give credit to me if you tell anyone and star this repo!.
Enjoy your badge! 🎉 If it stops working, feel free to ask for an update and I will try to fix it!
