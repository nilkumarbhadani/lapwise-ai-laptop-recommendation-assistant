# 🤖 NilBot — AI Laptop Recommendation Assistant

<div align="center">

![NilBot Banner](https://img.shields.io/badge/NilBot-AI%20Assistant-63b3ed?style=for-the-badge&logo=openai&logoColor=white)
![Deployed on Netlify](https://img.shields.io/badge/Deployed%20on-Netlify-00C7B7?style=for-the-badge&logo=netlify&logoColor=white)
![Powered by Flowise](https://img.shields.io/badge/Powered%20by-Flowise-7C3AED?style=for-the-badge)
![OpenRouter](https://img.shields.io/badge/LLM-OpenRouter-F59E0B?style=for-the-badge)

**An India-specific AI assistant that recommends the right laptop  
based on your budget and use case — in seconds.**

🔗 **[Live Demo → https://laptop-with-nil.netlify.app/](https://laptop-with-nil.netlify.app/)**

</div>

---

## 👋 Why I Built This

Every time someone around me asked *"which laptop should I buy?"* —  
I noticed the same frustration. Too many options, confusing specs, 
reviews that don't match Indian market prices, and no single honest advisor.

I built NilBot to fix that.

It asks you two simple questions — your budget and what you'll use the  
laptop for — and gives you a structured, honest recommendation with  
real INR pricing and an actual reason why each laptop fits your needs.  
No ads. No fluff. Just useful advice.

---

## ✨ Features

| Feature | Description |
|---|---|
| 🇮🇳 India-Specific | Real models available in India with accurate ₹ pricing |
| 🎯 Use-Case Driven | Coding · Gaming · Design/Video · Data Science · General College Work |
| 💬 Conversational | Supports follow-ups like "show me something lighter" or "under ₹60K?" |
| ⚖️ Honest Trade-Offs | Every recommendation includes one real limitation |
| 🌌 Premium Dark UI | Space theme with canvas particle animation & custom glowing cursor |
| 📱 Fully Responsive | Works cleanly on mobile, tablet, and desktop |
| 🔊 Sound Design | Subtle Web Audio API interaction sounds |
| ✨ Scroll Animations | Staggered fade-up reveals via Intersection Observer |
| 🔢 Animated Stats | Counter animates live on scroll entry |

---

## 🏗️ How It Works — The AI Pipeline

I built the entire AI flow visually using **Flowise** with 7 nodes:
Chat Input
↓
Welcome Node        → greets the user
↓
Budget Collection   → captures ₹ range
↓
Use Case Selection  → coding / gaming / design / data-science / general
↓
Prompt Node         → injects structured system prompt
↓
LLM Node            → OpenRouter processes the request
↓
Structured Output   → Name · Price · Specs · Why It Fits · Trade-Off

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| AI Pipeline | Flowise (Visual No-Code Builder) |
| LLM Provider | OpenRouter |
| Frontend | HTML · CSS · Vanilla JavaScript |
| Background Animation | Canvas API — 140-particle network |
| Scroll Animations | Intersection Observer API |
| Sound Effects | Web Audio API |
| Fonts | Syne · DM Sans |
| Deployment | Netlify |

---

## 🧠 My Prompt Engineering Approach

This was the part I spent the most time on.  
The system prompt enforces consistent, structured output every single time:
You are NilBot, an expert AI laptop recommendation assistant
for the Indian market.
For EACH laptop, output:

[Laptop Name + Model]
💰 Price: ₹XX,XXX (approx.)
⚙️ Specs: Processor | RAM | Storage | Display
✅ Why it fits: [1 sentence matching their use case]
⚠️ One trade-off: [honest limitation]

Rules:

Only recommend real, available laptops in India
Prices must reflect the Indian market accurately
Be concise, structured, and helpful
Ask for clarification if budget is unclear
Support follow-up questions naturally


**Decisions I made consciously:**

- **Structured format** → Forces the LLM to produce scannable, consistent output
- **India-specific constraint** → Prevents recommending products unavailable here
- **"One Trade-Off" rule** → My favourite decision. It makes the bot feel trustworthy, not salesy
- **Follow-up support** → Users can refine: "show me something lighter" or "anything under ₹60K?"

---

## 💬 Sample Conversation
Bot  → Hi! 👋 To suggest the best laptop for you, I just need:
your budget range and your primary use case.
User → Budget is ₹80,000. I need it for coding.
Bot  → Great! 🎯 Here are my top picks for coding at ₹80K:
   1. Lenovo IdeaPad Slim 5 (AMD Ryzen 7 7730U)
      💰 Price: ₹78,990
      ⚙️ Ryzen 7 | 16GB RAM | 512GB SSD | 15.6" IPS
      ✅ Why it fits: Handles VS Code, Docker, and multiple
         terminals without breaking a sweat.
      ⚠️ One trade-off: Integrated GPU only — not ideal 
         for casual gaming on the side.

   2. ASUS VivoBook 16X (Intel Core i5-12500H)
      ...
User → Can you show me something lighter?
Bot  → Sure! Here's a slimmer option in the same budget...

---

## 🎨 UI / UX Details

I wanted the frontend to feel like a real product, not a student project.  
Here's what I built into it:

- **Dark Space Theme** — Navy/midnight blue palette with cyan accent
- **Canvas Particle Network** — 140 animated particles with dynamic connection lines
- **Custom Glowing Cursor** — CSS `mix-blend-mode` with a lagging ring follower
- **Scroll-Reveal System** — Staggered `translateY` fade-up animations on entry
- **Animated Stat Counter** — Numbers count up from 0 on scroll
- **Responsive Typography** — CSS `clamp()` for fluid heading scaling
- **Web Audio Feedback** — Soft oscillator sounds on button interactions

---

## 🚀 Live Deployment

> 🔗 **[https://laptop-with-nil.netlify.app/](https://laptop-with-nil.netlify.app/)**

Deployed on **Netlify**. The Flowise chatbot widget is embedded via CDN —  
no backend server needed. Open it, type your budget, and try it yourself.

---

## ⚠️ Disclaimer

NilBot is an AI-powered assistant built for academic and educational purposes  
as part of a university assignment at **IIT Jodhpur**.  
Responses are generated by a large language model and may contain inaccuracies.  
Do not rely on this for final purchasing decisions without independent verification.  
Conversations may be processed by third-party providers (Flowise, OpenRouter).

---

## 👨‍💻 About Me

**Nil Kumar Bhadani**  
Student at IIT Jodhpur  
Building real AI products — not just tutorials.

I'm actively looking for opportunities in AI development,  
frontend engineering, and product-driven tech roles.  
Let's connect → [LinkedIn](https://www.linkedin.com/in/nil-kumar-bhadani-a57a10376/) · [GitHub](#)

---

<div align="center">

Built with 🤖 + ☕ by **Nil Kumar Bhadani** · IIT Jodhpur

⭐ If this project helped or inspired you, consider starring the repo!

</div>
