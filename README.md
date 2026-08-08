<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=32&duration=3000&pause=1000&color=6366F1&center=true&vCenter=true&width=800&height=80&lines=AI+Website+Builder;Build+Websites+with+AI;Turn+Ideas+Into+Websites;Powered+by+PERN+%2B+OpenRouter" alt="AI Website Builder" />

<br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:6366F1,50:8B5CF6,100:06B6D4&height=180&section=header&text=AI%20Website%20Builder&fontSize=42&fontColor=ffffff&animation=fadeIn&fontAlignY=45" width="100%" />

<br/>

<h2>🚀 Build Websites with Natural Language</h2>

<p>
  An AI-powered website builder that transforms your ideas into beautiful,<br/>
  responsive websites using <b>PERN</b>, <b>OpenRouter</b>, and modern web technologies.
</p>

<br/>

<img src="https://skillicons.dev/icons?i=react,typescript,vite,nodejs,express,postgres,prisma" />

<br/><br/>

<img src="https://img.shields.io/badge/OpenRouter-AI-6366F1?style=for-the-badge" />
<img src="https://img.shields.io/badge/Better%20Auth-Authentication-111827?style=for-the-badge" />
<img src="https://img.shields.io/badge/Stripe-Payments-635BFF?style=for-the-badge&logo=stripe&logoColor=white" />
<img src="https://img.shields.io/badge/Neon-PostgreSQL-00E599?style=for-the-badge&logo=postgresql&logoColor=white" />

<br/><br/>

<a href="https://github.com/Vedp6/Ai-Website-Builder">
  <img src="https://img.shields.io/github/stars/Vedp6/Ai-Website-Builder?style=for-the-badge" />
</a>

<a href="https://github.com/Vedp6/Ai-Website-Builder/fork">
  <img src="https://img.shields.io/github/forks/Vedp6/Ai-Website-Builder?style=for-the-badge" />
</a>

</div>

---

## 🌟 About The Project

**AI Website Builder** is a full-stack AI-powered platform that allows users to create websites using natural language.

Instead of manually writing HTML, CSS, and JavaScript, users can simply describe what they want and the AI generates the website.

### Example

> Create a modern portfolio website for a software developer with a dark theme, projects section, skills, and contact form.

The application uses **OpenRouter** to communicate with AI models, generates the website, stores projects in **Neon PostgreSQL** through **Prisma**, and provides a live preview.

---

## ✨ Features

### 🤖 AI Website Generation
- Generate websites using natural-language prompts
- AI-powered website/code generation
- OpenRouter integration
- Responsive website generation
- Live website preview
- Iterate on generated projects

### 🧑‍💻 Authentication
- User registration
- Email/password login
- Logout
- Persistent sessions
- Protected resources
- Better Auth integration
- Secure HTTP-only session cookies

### 📁 Project Management
- Create projects
- Save generated websites
- View previous projects
- Update projects
- Delete projects
- User-specific project data
- Persistent PostgreSQL storage

### 👀 Website Preview
- Live generated website preview
- Responsive preview
- Fast iteration
- Preview without leaving the builder

### 💳 Payments
- Stripe integration
- Secure payment processing
- Stripe webhook support
- Webhook verification
- Payment/subscription-ready architecture

### 🗄️ Database
- PostgreSQL
- Neon serverless PostgreSQL
- Prisma ORM
- Type-safe database access
- Persistent application data

### 🔐 Security
- Better Auth authentication
- Secure sessions
- HTTP-only cookies
- HTTPS support
- CORS protection
- Environment-based secrets
- Stripe webhook verification
- Protected API routes

---

# 🛠️ Tech Stack

<div align="center">

### Frontend

<img src="https://skillicons.dev/icons?i=react,typescript,vite,tailwind" />

### Backend

<img src="https://skillicons.dev/icons?i=nodejs,express,typescript" />

### Database & ORM

<img src="https://skillicons.dev/icons?i=postgres,prisma" />

### AI, Authentication & Payments

<br/>

<img src="https://img.shields.io/badge/OpenRouter-AI-6366F1?style=for-the-badge" />
<img src="https://img.shields.io/badge/Better%20Auth-Authentication-111827?style=for-the-badge" />
<img src="https://img.shields.io/badge/Stripe-Payments-635BFF?style=for-the-badge&logo=stripe&logoColor=white" />
<img src="https://img.shields.io/badge/Neon-PostgreSQL-00E599?style=for-the-badge&logo=postgresql&logoColor=white" />

### Deployment

<img src="https://skillicons.dev/icons?i=vercel,github" />

<br/>

<img src="https://img.shields.io/badge/Backend-Render-46E3B7?style=for-the-badge" />

</div>

---

# 🏗️ Architecture

```text
                    ┌─────────────────────────┐
                    │          USER           │
                    │   Natural Language      │
                    │         Prompt          │
                    └────────────┬────────────┘
                                 │
                                 ▼
                    ┌─────────────────────────┐
                    │      React + Vite       │
                    │       Frontend          │
                    │         Vercel          │
                    └────────────┬────────────┘
                                 │
                          HTTPS API Requests
                                 │
                                 ▼
                    ┌─────────────────────────┐
                    │    Node.js + Express    │
                    │        Backend          │
                    │         Render          │
                    └──────┬──────┬───────┬───┘
                           │      │       │
             ┌─────────────┘      │       └─────────────┐
             ▼                    ▼                     ▼
      ┌─────────────┐     ┌─────────────┐       ┌─────────────┐
      │ Better Auth │     │   Prisma    │       │ OpenRouter  │
      │             │     │     ORM     │       │     AI      │
      └─────────────┘     └──────┬──────┘       └─────────────┘
                                  │
                                  ▼
                         ┌────────────────┐
                         │      Neon      │
                         │   PostgreSQL   │
                         └────────────────┘

                                  │
                                  ▼
                           ┌─────────────┐
                           │   Stripe    │
                           │  Payments   │
                           └─────────────┘
```

---

# 📂 Project Structure

```text
AI-Website-Builder/
│
├── Client/
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── hooks/
│   │   ├── lib/
│   │   ├── services/
│   │   └── ...
│   ├── package.json
│   └── ...
│
├── Server/
│   ├── controllers/
│   │   ├── projectController.ts
│   │   ├── stripeWebhook.ts
│   │   └── userController.ts
│   │
│   ├── routes/
│   │   ├── projectRoutes.ts
│   │   └── userRoutes.ts
│   │
│   ├── middlewares/
│   │   └── auth.ts
│   │
│   ├── lib/
│   │   ├── auth.ts
│   │   └── prisma.ts
│   │
│   ├── prisma/
│   │   ├── schema.prisma
│   │   └── migrations/
│   │
│   ├── server.ts
│   ├── package.json
│   └── ...
│
└── README.md
```

---

# 🔄 How It Works

### 1️⃣ User enters a prompt

```text
Create a modern SaaS landing page
for an AI startup with pricing,
features and a dark theme.
```

### 2️⃣ Frontend sends the request

```text
React
  ↓
Express API
```

### 3️⃣ Backend communicates with AI

```text
Express
   ↓
OpenRouter
   ↓
AI Model
```

### 4️⃣ AI generates the website

The generated result is returned to the backend and displayed to the user.

### 5️⃣ Project is saved

```text
Express
   ↓
Prisma
   ↓
Neon PostgreSQL
```

### 6️⃣ User sees the result

The frontend displays the generated website in the preview interface.

---

# 🔐 Authentication Flow

```text
User
 │
 ▼
React Frontend
 │
 ▼
Better Auth
 │
 ▼
Express Backend
 │
 ▼
Prisma
 │
 ▼
Neon PostgreSQL
```

Better Auth provides:
- Registration
- Login
- Logout
- Sessions
- Protected resources
- Secure authentication cookies

---

# 💳 Stripe Payment Flow

```text
User
 │
 ▼
Frontend
 │
 ▼
Backend
 │
 ▼
Stripe Checkout
 │
 ▼
Payment
 │
 ▼
Stripe Webhook
 │
 ▼
Backend
 │
 ▼
Database
```

Stripe webhook events are verified on the backend before payment-related data is processed.

---

# 🗄️ Database

The project uses **PostgreSQL + Neon + Prisma**.

```text
Users
  │
  ├── Authentication
  │
  └── Projects
        ├── Project details
        ├── Generated content
        └── Website data
```

Prisma provides:
- Type-safe queries
- Database migrations
- Schema management
- PostgreSQL integration

---

# ⚙️ Environment Variables

## Server

Create a `.env` file:

```env
TRUSTED_ORIGIN=https://your-frontend.vercel.app
DATABASE_URL=your_neon_database_url

BETTER_AUTH_SECRET=your_better_auth_secret
BETTER_AUTH_URL=https://your-backend.onrender.com

NODE_ENV=production

STRIPE_SECRET_KEY=your_stripe_secret_key
STRIPE_WEBHOOK_SECRET=your_stripe_webhook_secret

OPENROUTER_API_KEY=your_openrouter_api_key
```

## Client

```env
VITE_BASEURL=https://your-backend.onrender.com
```

> ⚠️ Never commit `.env` files or private API keys to GitHub.

---

# 🚀 Local Development

## Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git
cd YOUR_REPOSITORY
```

## Backend Setup

```bash
cd Server
npm install
```

Create your `.env` file and configure the required environment variables.

Generate Prisma Client:

```bash
npx prisma generate
```

Run migrations:

```bash
npx prisma migrate dev
```

Start the backend:

```bash
npm run server
```

## Frontend Setup

```bash
cd Client
npm install
```

Create:

```env
VITE_BASEURL=http://localhost:3000
```

Start the frontend:

```bash
npm run dev
```

---

# 🌐 Deployment

### Frontend — Vercel

```text
React + Vite
      ↓
    Vercel
```

### Backend — Render

```text
Node.js + Express + TypeScript
      ↓
    Render
```

### Database — Neon

```text
PostgreSQL
    ↓
   Neon
```

### AI — OpenRouter

```text
Backend
   ↓
OpenRouter
   ↓
AI Model
```

### Payments — Stripe

```text
Backend
   ↓
Stripe
   ↓
Webhook
```

---

# 📦 Production Backend Commands

Build:

```bash
npm install --include=dev && npx prisma generate && npm run build
```

Start:

```bash
npm start
```

---

# 🔒 Security Considerations

- API keys are stored in environment variables
- Authentication is handled through Better Auth
- Session cookies are protected
- HTTPS is used in production
- CORS is configured for trusted origins
- Stripe webhooks are verified
- Database credentials are never exposed to the frontend
- OpenRouter API keys remain server-side
- Protected API routes require authentication

---

# 🧠 AI Architecture

```text
User Prompt
     │
     ▼
React UI
     │
     ▼
Express API
     │
     ▼
OpenRouter
     │
     ▼
Selected AI Model
     │
     ▼
Generated Website
     │
     ├──────────────► Save with Prisma
     │                     │
     │                     ▼
     │                    Neon
     │
     ▼
Live Preview
```

---

# 📸 Screenshots

Add screenshots of your application here:

```text
docs/
├── dashboard.png
├── ai-generator.png
├── preview.png
├── projects.png
└── payment.png
```

Example:

```md
![Dashboard](./docs/dashboard.png)
```

---

# 📈 Future Improvements

- [ ] Multi-model AI selection
- [ ] AI-powered website editing
- [ ] Drag-and-drop editor
- [ ] Custom domain support
- [ ] One-click website deployment
- [ ] GitHub integration
- [ ] Website templates
- [ ] Version history
- [ ] Team collaboration
- [ ] AI image generation
- [ ] AI-powered SEO optimization
- [ ] Custom code export
- [ ] Website analytics

---

# 🤝 Contributing

Contributions are welcome!

1. Fork the repository
2. Create a new branch

```bash
git checkout -b feature/amazing-feature
```

3. Make your changes
4. Commit your changes

```bash
git commit -m "Add amazing feature"
```

5. Push to your branch

```bash
git push origin feature/amazing-feature
```

6. Open a Pull Request

---

# ⭐ Support

If you found this project useful, consider giving it a ⭐ on GitHub!

---

<div align="center">

## ⚡ Built With

<img src="https://skillicons.dev/icons?i=react,typescript,vite,nodejs,express,postgres,prisma,github,vercel" />

<br/><br/>

<img src="https://img.shields.io/badge/OpenRouter-AI-6366F1?style=for-the-badge" />
<img src="https://img.shields.io/badge/Neon-PostgreSQL-00E599?style=for-the-badge" />
<img src="https://img.shields.io/badge/Better%20Auth-Authentication-111827?style=for-the-badge" />
<img src="https://img.shields.io/badge/Stripe-Payments-635BFF?style=for-the-badge&logo=stripe&logoColor=white" />

<br/><br/>

**Made with ❤️ using AI + PERN**

</div>
