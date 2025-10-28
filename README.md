# 🌟 Giya AI

<div align="center">

![Giya AI Banner](https://via.placeholder.com/1200x300/6366f1/ffffff?text=Giya+AI+-+Your+AI-Powered+Career+Companion)

**Where AI Meets Career Intelligence**

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Status](https://img.shields.io/badge/status-active-success.svg)]()
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

[Live Demo](https://giya-ai.com) • [Documentation](https://docs.giya-ai.com) • [Report Bug](https://github.com/yourusername/giya-ai/issues) • [Request Feature](https://github.com/yourusername/giya-ai/issues)

</div>

---

## 🎯 What is Giya AI?

**Giya AI** is a collaborative platform where students and professionals get AI-powered guidance for career decisions and project planning. Think of it as **"ChatGPT for career counseling + group brainstorming."**

### 💡 The Problem We Solve

- Students struggle to navigate career paths without personalized guidance
- Professionals need smart tools for project planning and collaboration
- Career counseling is expensive and often inaccessible
- Generic advice doesn't account for individual strengths and market trends

### ✨ Our Solution

Giya AI combines cutting-edge AI technology with real-time collaboration to provide:
- **Personalized career roadmaps** based on your unique profile
- **AI-powered brainstorming sessions** for teams and individuals
- **Industry insights** using live data and market trends
- **Interactive storytelling** that visualizes your future career path

---

## 🚀 Key Features

<table>
<tr>
<td width="50%">

### 🤖 AI Chat Assistant (@GiyaAI)
Intelligent conversational AI that understands context and provides actionable career advice. Mention `@GiyaAI` in any channel for instant guidance.

</td>
<td width="50%">

### 🧭 Career Compass
Take a comprehensive assessment that analyzes your skills, interests, and goals to generate a personalized career roadmap with learning paths.

</td>
</tr>
<tr>
<td width="50%">

### 📖 Narrative Generation
Experience your future career through AI-generated stories. See yourself succeeding in different roles and industries through immersive storytelling.

</td>
<td width="50%">

### 👥 Real-Time Collaboration
Work together with peers, mentors, and AI in shared workspaces. Brainstorm ideas, plan projects, and make decisions collaboratively.

</td>
</tr>
<tr>
<td width="50%">

### 📊 Industry Intelligence
Access up-to-date market data, job trends, and skill demands powered by Google Search API and real-time data analysis.

</td>
<td width="50%">

### 🎓 Learning Pathways
Get curated learning resources, courses, and milestones tailored to your career goals and current skill level.

</td>
</tr>
</table>

---

## 🏗️ Architecture

```
┌─────────────────────────────────────────────────────────────┐
│                         Frontend                             │
│                    (Figma → Framer/React)                    │
│                                                               │
│  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐         │
│  │   Chat UI   │  │   Career    │  │  Narrative  │         │
│  │             │  │   Compass   │  │   Viewer    │         │
│  └─────────────┘  └─────────────┘  └─────────────┘         │
└─────────────────────────────────────────────────────────────┘
                            │
                    API Calls (REST/GraphQL)
                            │
┌─────────────────────────────────────────────────────────────┐
│                    Backend API Layer                         │
│                  (Node.js/Express/Serverless)                │
│                                                               │
│  ┌──────────────┐  ┌──────────────┐  ┌──────────────┐      │
│  │ Chat Handler │  │ Career Logic │  │Story Generator│      │
│  └──────────────┘  └──────────────┘  └──────────────┘      │
└─────────────────────────────────────────────────────────────┘
                            │
              ┌─────────────┴─────────────┐
              │                           │
    ┌─────────▼────────┐       ┌─────────▼────────┐
    │   Gemini API     │       │  Google Search   │
    │  (AI Processing) │       │    API (Data)    │
    └──────────────────┘       └──────────────────┘
              │
    ┌─────────▼────────┐
    │   Supabase       │
    │ (Database + Auth)│
    └──────────────────┘
```

---

## 🛠️ Tech Stack

### Frontend
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![Framer](https://img.shields.io/badge/Framer-0055FF?style=for-the-badge&logo=framer&logoColor=white)

### Backend
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![Express](https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-181818?style=for-the-badge&logo=supabase&logoColor=white)

### AI & Data
![Google Gemini](https://img.shields.io/badge/Google_Gemini-4285F4?style=for-the-badge&logo=google&logoColor=white)
![Google Search API](https://img.shields.io/badge/Google_Search-4285F4?style=for-the-badge&logo=google&logoColor=white)

### DevOps
![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2CA5E0?style=for-the-badge&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white)

---

## 🎬 Getting Started

### Prerequisites

```bash
node >= 18.0.0
npm >= 9.0.0
```

### Installation

1. **Clone the repository**
```bash
git clone https://github.com/yourusername/giya-ai.git
cd giya-ai
```

2. **Install dependencies**
```bash
npm install
```

3. **Set up environment variables**
```bash
cp .env.example .env
```

Edit `.env` with your credentials:
```env
GEMINI_API_KEY=your_gemini_api_key
GOOGLE_SEARCH_API_KEY=your_google_search_key
SUPABASE_URL=your_supabase_url
SUPABASE_ANON_KEY=your_supabase_anon_key
```

4. **Run the development server**
```bash
npm run dev
```

5. **Open your browser**
Navigate to `http://localhost:3000`

---

## 📚 Documentation

### API Endpoints

#### Chat Endpoints
```
POST   /api/chat              # Send a message to AI
GET    /api/chat/:channelId   # Get chat history
```

#### Career Compass
```
POST   /api/career/assess     # Submit career assessment
GET    /api/career/profile    # Get user career profile
POST   /api/career/narrative  # Generate career narrative
```

#### User Management
```
POST   /api/auth/signup       # Create new account
POST   /api/auth/login        # User login
GET    /api/users/profile     # Get user profile
```

### Environment Variables

| Variable | Description | Required |
|----------|-------------|----------|
| `GEMINI_API_KEY` | Google Gemini API key | ✅ |
| `GOOGLE_SEARCH_API_KEY` | Google Search API key | ✅ |
| `SUPABASE_URL` | Supabase project URL | ✅ |
| `SUPABASE_ANON_KEY` | Supabase anonymous key | ✅ |
| `PORT` | Server port (default: 3000) | ❌ |

---

## 🤝 Contributing

We love contributions! Here's how you can help:

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct and the process for submitting pull requests.

---

## 🗺️ Roadmap

- [x] AI Chat Assistant with context awareness
- [x] Career Compass assessment tool
- [x] Narrative generation engine
- [ ] Mobile app (iOS & Android)
- [ ] Voice interaction support
- [ ] Multi-language support (German, Spanish, French)
- [ ] Mentor matching system
- [ ] Job board integration
- [ ] Premium analytics dashboard
- [ ] API for third-party integrations

See the [open issues](https://github.com/yourusername/giya-ai/issues) for a full list of proposed features and known issues.

---

## 📊 Project Stats

<div align="center">

![GitHub stars](https://img.shields.io/github/stars/yourusername/giya-ai?style=social)
![GitHub forks](https://img.shields.io/github/forks/yourusername/giya-ai?style=social)
![GitHub watchers](https://img.shields.io/github/watchers/yourusername/giya-ai?style=social)

</div>

---

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 💖 Acknowledgments

- **Google Gemini** for providing powerful AI capabilities
- **Supabase** for the amazing backend infrastructure
- **Open Source Community** for inspiration and support
- **Our Users** for valuable feedback and feature requests

---

## 📞 Contact

**Project Maintainer:** Your Name

- Email: your.email@example.com
- LinkedIn: [Your LinkedIn](https://linkedin.com/in/yourprofile)
- Twitter: [@yourhandle](https://twitter.com/yourhandle)

**Project Link:** [https://github.com/yourusername/giya-ai](https://github.com/yourusername/giya-ai)

---

<div align="center">

### 🌟 Star us on GitHub — it motivates us a lot!

Made with ❤️ by the Giya AI Team

[⬆ back to top](#-giya-ai)

</div>
