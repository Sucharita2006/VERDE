# VERDE Dashboard 🌱

The B2B SaaS platform that empowers restaurants and cafes to effortlessly transition their menus toward profitable, plant-based alternatives. 

**VERDE (Vegetarian Evolving Restaurant & Dining Ecosystem)** acts as an AI co-pilot for restaurant owners. From automatically reformulating existing recipes to finding local suppliers and generating Instagram-ready marketing videos, VERDE handles the heavy lifting of modernizing a restaurant's menu for the growing flexitarian audience.

---

## ✨ Features

### 🤖 AI Recipe Reformulation
Automatically analyze any existing meat or dairy-based dish and generate a plant-based alternative. 
- Matches **Taste & Texture** profiles.
- Optimizes **Nutrition** (protein parity using pea/soy isolates).
- Computes **Raw Material Costs** and suggests ingredient substitutions.

### 🎥 AI Marketing Agent (Video Reels)
Turn a dish into an Instagram-ready marketing campaign in seconds.
- Uses **Fal.ai (Kling 1.5 Pro)** to generate cinematic 10-second vertical video reels of the food.
- Generates engaging captions and trending hashtags automatically based on daily food trends.
- Users can customize the reels via an intuitive chat interface.

### 📦 Supplier & Procurement Matching
Stop guessing where to buy plant-based ingredients.
- Automatically searches for local and online suppliers for niche ingredients (e.g., Pea Protein Isolate, Nutritional Yeast, Vegan Cheese).
- Provides live pricing, stock availability, and direct purchase links.
- Uses **Genkit** and **OpenRouter (Google Gemini)** combined with live web search APIs.

### 💳 Subscription Management
A fully integrated, tiered subscription model built for scale.
- **Starter, Growth, and Pro** tiers.
- Integrated with **Razorpay** for seamless payments and webhook-based subscription tracking.
- Hard limits and usage tracking for AI credits (Dish Analyses, Marketing Generations, Video Reels).

### 💬 Sprout App Integration
The dashboard connects directly to the **Sprout Consumer App**, allowing owners to:
- Receive and manage live orders.
- Manage table reservations.
- View and reply to customer reviews.

---

## 🛠 Tech Stack

- **Framework:** [Next.js 15](https://nextjs.org/) (App Router, React Server Components, Server Actions)
- **Language:** TypeScript
- **Styling:** Tailwind CSS & [shadcn/ui](https://ui.shadcn.com/)
- **Database & Auth:** [Supabase](https://supabase.com/)
- **AI Orchestration:** [Firebase Genkit](https://firebase.google.com/docs/genkit)
- **AI Models:** Google Gemini 2.5 Pro (via OpenRouter)
- **Video Generation:** [Fal.ai](https://fal.ai/) (Kling 1.5 Pro)
- **Payments:** Razorpay

---

## 🚀 Getting Started

### Prerequisites
- Node.js (v18+)
- A Supabase project
- API Keys for: Razorpay, OpenRouter (Gemini), and Fal.ai.

### 1. Clone the repository
```bash
git clone https://github.com/your-username/verde.git
cd verde/verde2
```

### 2. Install dependencies
```bash
npm install
# or
yarn install
```

### 3. Setup Environment Variables
Copy the `.env.example` file to `.env.local` and fill in your keys:
```bash
cp .env.example .env.local
```

### 4. Run the development server
```bash
npm run dev
# or
yarn dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the dashboard.

---

## 🔒 Security Note
This repository contains no hardcoded API keys or secrets. All sensitive configurations are managed securely via environment variables and Supabase Row Level Security (RLS) policies.

---

*Built for the future of food.* 🌍
