# 🤖 MY AI Bot - Intelligent Chat Assistant

<div align="center">

[![Next.js](https://img.shields.io/badge/Next.js-15.5.4-black?style=for-the-badge&logo=next.js)](https://nextjs.org/)
[![React](https://img.shields.io/badge/React-19.2.0-blue?style=for-the-badge&logo=react)](https://reactjs.org/)
[![Google Gemini](https://img.shields.io/badge/Google-Gemini_2.0_Flash-4285F4?style=for-the-badge&logo=google)](https://ai.google.dev/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.0-blue?style=for-the-badge&logo=typescript)](https://www.typescriptlang.org/)

*A modern, intelligent AI chat assistant powered by Google's Gemini 2.0 Flash model*

[Live Demo](#) • [Features](#-features) • [Installation](#-installation) • [Usage](#-usage)

</div>

---

## 🚀 Features

### ✨ **Smart Conversations**
- 💬 Real-time chat with Google's latest Gemini 2.0 Flash model
- 🔄 Streaming responses for instant interaction
- 🧠 Context-aware conversations that remember your chat history

### 🎨 **Beautiful Interface**
- 🌙 Modern dark/light theme support
- 📱 Fully responsive design for all devices
- ⚡ Lightning-fast performance with Next.js 15 and Turbopack
- 🎯 Intuitive chat interface with sidebar navigation

### 🛠️ **Advanced Features**
- 📝 Markdown support for rich text formatting
- 🔧 Sidebar with conversation threads
- ⌨️ Keyboard shortcuts for power users
- 🎪 Smooth animations with Framer Motion
- 🔄 Auto-save conversations

### 🔒 **Secure & Reliable**
- 🔐 Environment-based API key management
- 🚀 Built with TypeScript for type safety
- 📊 Error handling and loading states
- 🏗️ Scalable architecture

---

## 🎯 What Makes This Special?

This isn't just another chatbot! Here's what sets MY AI Bot apart:

- **🔥 Latest AI Technology**: Powered by Google's Gemini 2.0 Flash - the most advanced conversational AI
- **⚡ Real-time Streaming**: See responses as they're generated, not after completion
- **🎨 Premium UI/UX**: Built with modern React patterns and beautiful animations
- **📱 Mobile-First**: Perfect experience on any device, anywhere
- **🔧 Developer-Friendly**: Clean, maintainable code with TypeScript

---

## 🛠️ Installation

### Prerequisites
- Node.js 18+ 
- npm, yarn, or pnpm
- Google AI API Key ([Get one here](https://makersuite.google.com/app/apikey))

### Quick Start

1. **Clone the repository**
```bash
git clone https://github.com/rituraj000/MY-AI-bot.git
cd MY-AI-bot
```

2. **Install dependencies**
```bash
npm install
# or
yarn install
# or
pnpm install
```

3. **Set up environment variables**
```bash
cp .env.example .env.local
```

Edit `.env.local` and add your Google AI API key:
```env
GOOGLE_GENERATIVE_AI_API_KEY=your_api_key_here
```

4. **Start the development server**
```bash
npm run dev
```

5. **Open your browser**
Navigate to [http://localhost:3000](http://localhost:3000) and start chatting!

---

## 🎮 Usage

### Basic Chat
1. Type your message in the input box
2. Press Enter or click Send
3. Watch as the AI responds in real-time!

### Advanced Features
- **📁 Sidebar Navigation**: Access previous conversations
- **⌨️ Keyboard Shortcuts**: Use `Ctrl/Cmd + B` to toggle sidebar
- **📝 Markdown**: The AI supports **bold**, *italic*, `code`, and more!

### Example Conversations
```
You: "Explain quantum computing in simple terms"
AI: "Quantum computing is like having a super-powered computer that can..."

You: "Write a Python function to sort a list"
AI: "```python
def sort_list(items):
    return sorted(items)
```"
```

---

## 🔧 Configuration

### Environment Variables

| Variable | Description | Required |
|----------|-------------|----------|
| `GOOGLE_GENERATIVE_AI_API_KEY` | Your Google AI API key | ✅ |

### Customization

Want to customize the AI behavior? Edit `app/api/chat/route.ts`:

```typescript
const result = streamText({
  model: google("gemini-2.0-flash"),
  messages: convertToModelMessages(messages),
  // Add custom parameters here
  temperature: 0.7,
  maxTokens: 1000,
});
```

---

## 🚀 Deployment

### Deploy on Vercel (Recommended)

1. Push your code to GitHub
2. Connect your repository to [Vercel](https://vercel.com)
3. Add your environment variables in Vercel dashboard
4. Deploy! 🎉

### Other Platforms

This app can be deployed on any platform that supports Next.js:
- **Netlify**
- **Railway**
- **Heroku**
- **AWS**
- **Google Cloud Platform**

---

## 🎨 Tech Stack

- **Framework**: Next.js 15 with App Router
- **Frontend**: React 19, TypeScript 5
- **AI SDK**: Vercel AI SDK with Google AI provider
- **Styling**: Tailwind CSS, Radix UI components
- **Animations**: Framer Motion
- **Build Tool**: Turbopack for lightning-fast builds

---

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

- **Google AI** for the incredible Gemini model
- **Vercel** for the AI SDK and Next.js framework
- **Assistant UI** for the beautiful chat components
- **The open-source community** for making this possible

---

<div align="center">

**Made with ❤️ by [rituraj000](https://github.com/rituraj000)**

⭐ **Star this repo if you found it helpful!** ⭐

[Report Bug](https://github.com/rituraj000/MY-AI-bot/issues) • [Request Feature](https://github.com/rituraj000/MY-AI-bot/issues) • [Documentation](https://github.com/rituraj000/MY-AI-bot/wiki)

</div>
