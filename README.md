# Social Media Workflow

An AI-powered multi-platform social media automation system built with n8n, enabling automatic content generation and publishing across multiple social channels.

## ✨ Key Features

- 🤖 **AI Content Generation** - Automatic content creation using LLMs
- 📱 **Multi-Platform Support** - LinkedIn, Instagram, Facebook, Twitter, TikTok, Threads, YouTube Shorts
- 🎨 **Image Generation** - AI-powered image creation for posts
- 📅 **Scheduling** - Schedule posts for optimal engagement
- ✅ **Approval Gate** - Review content before publishing
- 📊 **Analytics** - Track performance and engagement
- 🔐 **Secure Credentials** - Environment-based credential management

## 🛠️ Technology Stack

- **n8n** - Workflow automation platform
- **Google Gemini** - LLM for content generation
- **OpenAI GPT-4o** - Advanced language model
- **SerpAPI** - Research augmentation
- **IMGBB** - Image hosting
- **Social Media APIs** - Platform integrations

## 📦 Installation

### Option 1: n8n Cloud
1. Create account at [n8n.io](https://n8n.io)
2. Import the workflow JSON
3. Configure credentials
4. Add environment variables

### Option 2: Docker (Production)

```bash
# Clone the repository
git clone https://github.com/Abhishekj9621/Social-Media-Workflow.git
cd Social-Media-Workflow

# Create .env file
cp .env.example .env

# Edit .env with your API keys
nano .env

# Start services
docker-compose up -d
```

## 🚀 Quick Start

1. Set up n8n instance
2. Import workflow from JSON file
3. Configure all required credentials
4. Add API keys to environment variables
5. Submit topic via form
6. Review generated content
7. Approve and publish

## 📁 Project Structure

```
Social-Media-Workflow/
├── workflows/
│   └── social-media-automation.json
├── .env.example
├── docker-compose.yml
├── README.md
└── .gitignore
```

## 🔄 Workflow Architecture

```
Form Trigger (Topic Input)
        ↓
AI Content Agent (Gemini + GPT-4o)
        ↓
Platform-Specific Content Generation
├── LinkedIn (Professional tone)
├── Instagram (Visual storytelling)
├── Facebook (Community-based)
├── Twitter (Concise)
├── TikTok (Short video)
├── Threads (Conversational)
└── YouTube Shorts (Tutorial)
        ↓
Image Generation (OpenAI)
        ↓
Image Hosting (IMGBB)
        ↓
Approval Gate (Boolean check)
        ↓
Auto Publishing to All Platforms
```

## 🔧 Core Components

### AI Content Agent
- Multi-LLM hybrid design
- Structured JSON output
- Platform-specific tone optimization
- Automated hashtag generation

### Image Generation
- OpenAI image generation
- Prompt derived from content
- Automated formatting

### Publishing Engine
- Multi-platform simultaneous publishing
- Error handling and retry logic
- Status tracking

## 💻 Environment Variables

Create `.env` file:

```env
# OpenAI
OPENAI_API_KEY=sk-xxx

# Google
GOOGLE_API_KEY=xxx

# SerpAPI
SERPAPI_API_KEY=xxx

# IMGBB
IMGBB_API_KEY=xxx

# Social Media Credentials
TWITTER_API_KEY=xxx
FACEBOOK_TOKEN=xxx
LINKEDIN_TOKEN=xxx
INSTAGRAM_TOKEN=xxx
```

## 📊 Platform Configuration

| Platform | Tone | Format | CTA |
|----------|------|--------|-----|
| LinkedIn | Professional | 3-4 sentences | Comment-driven |
| Instagram | Visual storytelling | Caption + hashtags | Engagement |
| Facebook | Community | Conversational | Share & comment |
| Twitter | Concise | <150 chars | Reply/Retweet |
| TikTok | Trendy | 15-60 sec script | Follow tips |
| Threads | Conversational | Discussion-style | Questions |
| YouTube Shorts | Tutorial | <60 seconds | Subscribe |

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/improvement`)
3. Commit your changes (`git commit -am 'Add new feature'`)
4. Push to the branch (`git push origin feature/improvement`)
5. Open a Pull Request

## ⚠️ Security Best Practices

- Never commit `.env` file
- Add `.env` to `.gitignore`
- Regenerate exposed API keys immediately
- Use environment variables for all secrets
- Rotate credentials regularly

## 🔮 Future Enhancements

- Content calendar
- A/B testing
- Performance analytics
- Multi-client support
- SaaS dashboard
- Scheduling layer

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 👤 Author

**Abhishek Jaiswal**  
Email: aj962143@gmail.com

---

For more information and documentation, visit the [GitHub repository](https://github.com/Abhishekj9621/Social-Media-Workflow)