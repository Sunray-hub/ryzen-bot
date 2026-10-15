# 🐉 Ryzen — Your AI-Powered Discord Companion

<div align="center">

<a href="https://github.com/Sunray-hub">
<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=700&size=30&pause=1000&color=00D9FF&center=true&vCenter=true&width=600&height=80&lines=Meet+Ryzen+%F0%9F%90%89;AI+for+your+Discord+server;Your+server.+Your+API+key.;Powered+by+Google+Gemini." alt="Ryzen animated title" />
</a>

**One bot. Your server. Your own Gemini API key.**

Ryzen is a Discord AI chatbot hosted on my own server. Invite it to your community, configure your Gemini API key, and you're ready to go!

[![Discord.py](https://img.shields.io/badge/Discord.py-Bot-5865F2?style=for-the-badge&logo=discord)](https://discordpy.readthedocs.io/)
[![Google Gemini](https://img.shields.io/badge/Powered%20by-Gemini-8E75B2?style=for-the-badge&logo=googlegemini)](https://ai.google.dev/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)
[![Hosted](https://img.shields.io/badge/Hosting-Self--Hosted-00D9FF?style=for-the-badge&logo=linux&logoColor=black)](https://github.com/Sunray-hub)

</div>

---

## ✨ What makes Ryzen different?

- 🧠 **AI-powered conversations** using Google Gemini.
- 🔑 **Bring your own API key:** each Discord server configures its own key.
- 🔐 **Encrypted API key storage** on the host server.
- 🔄 **Automatic model fallback** when supported errors occur.
- 💬 **Natural replies** with optional message replies and emoji reactions.
- 🛡️ **Channel controls** so moderators can decide where Ryzen responds.
- ⚡ **No installation required:** no Python, Docker, or server setup for your community.

## 🚀 How to get started

### 1. Invite Ryzen

Use the official invite link provided by the project owner.

> Invite link coming soon.

### 2. Get a Gemini API key

Visit [Google AI Studio](https://aistudio.google.com/) and obtain your own Gemini API key. Check the current API terms, availability, and usage limits.

Each server uses its own key, so its Gemini usage is associated with that key.

### 3. Run `/setup`

A server administrator with **Manage Server** permission runs `/setup` and submits the Gemini API key through Ryzen's private setup form.

Ryzen verifies the key, encrypts it, and saves it for that Discord server.

### 4. Start chatting!

That's it! Send a message in a channel where Ryzen is enabled, and it can respond using your server's configured Gemini API key.

## 🔐 How API keys work

Ryzen runs on a server maintained by the project owner. Discord server administrators provide their own Gemini API keys through `/setup`.

1. Ryzen receives the key through a private Discord interaction.
2. It attempts to verify that the key works.
3. It encrypts the key using Fernet.
4. It stores the encrypted key in the host's server configuration.
5. When your server sends a message, Ryzen decrypts the corresponding key and uses it to request a Gemini response.

**Important:** Encryption protects stored keys, but the bot host still needs access to decrypt them when making API requests. Only provide keys you are comfortable using with this hosted service.

## 🛠️ Available commands

| Command | Description | Permission |
|---|---|---|
| `/setup` | Configure Ryzen with your Gemini API key | Manage Server |
| `/blockchannel` | Stop Ryzen from responding in the current channel | Manage Channels |
| `/unblockchannel` | Allow Ryzen to respond in the current channel | Manage Channels |

## 💡 Who pays for AI usage?

Each Discord server supplies its own Gemini API key. AI requests made using that key count against the applicable Google API quota and billing arrangements for that key.

Ryzen's hosting is maintained separately by the project owner. Hosting availability depends on the server running and maintaining its connection to Discord.

## 📜 License

Ryzen is licensed under the [MIT License](LICENSE).

## 🐉 Join the Ryzen community

Have ideas, found a bug, or want to help improve Ryzen? Open an issue in this repository.
Or join the discord a issue a ticket: https://discord.com/invite/RarqvuNpQR

<div align="center">

**Your community. Your API key. Your Ryzen.** 🐉

</div>
