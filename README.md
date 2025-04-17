# 💬 DiscordOps – Real-Time Discord Agent with Web Search

**DiscordOps** is a high-performance, real-time communication agent powered by **Groq** and built with **Agno**, designed to interact with Discord servers using natural language. Equipped with Discord tools and DuckDuckGo search, it allows you to control server actions like reading/sending messages, managing threads, reactions, and more — all from a simple chat UI.

---

## 🚀 Installation & Running

### 1. Setup Environment Variables

Create a `.env` file based on `.env.example` and fill in:

- `GROQ_API_KEY` – Your Groq API key
- `DISCORD_BOT_TOKEN` – Your Discord bot token

---

### 2. Clone MCP Discord Server Integration

```bash
git clone https://github.com/barryyip0625/mcp-discord.git
cd mcp-discord

# Install dependencies
npm install

# Compile TypeScript
npm run build
```

---

### 3. Prepare Python Environment

```bash
uv venv
uv sync
```

---

### 4. Clone & Run the Agent UI

```bash
npx create-agent-ui@latest
# Enter 'y' when prompted to create a new project
# Follow the CLI to install dependencies
```

---

### 5. Start the Agent Backend

```bash
uv run main.py
```

---

### 6. Start the Agent UI

In a separate terminal:

```bash
cd agent-ui
npm run dev
```

---

### 7. Start Using DiscordOps

- Open your browser and go to: `http://localhost:3000`
- Input the **Channel ID** where your bot is present.
- Use natural language commands to:
  - Read or send messages
  - React to messages
  - Create or manage threads
  - Perform web searches and post results to Discord

---

## 🧠 Example Commands

- "Read the last 5 messages from #general"
- "Send 'Hey everyone!' to channel ID 1234567890"
- "Search 'latest Valorant patch notes' and send to #gaming-news"
- "React to the last message in #feedback with 👍"

---

## 🧩 Notes

- This agent is **on-demand**, not always active. It performs actions only when you prompt it through the chat UI.
- You must provide a valid **Channel/Guild ID** where your bot has access.
