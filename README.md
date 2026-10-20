# Vedottam (वेदोत्तम) - AI Spiritual Guide 🪔

Vedottam is an AI-powered Retrieval-Augmented Generation (RAG) application designed to bridge the gap between ancient Sanatan Dharma wisdom and modern-day challenges. It acts as a contextual spiritual guide, retrieving relevant *shlokas* (verses) from the Bhagavad Gita based on user queries (e.g., anxiety, career stress, moral dilemmas) and explaining them in a simple, modern tone.

## 🚀 Features

- **Semantic Search (RAG Engine):** Uses vector embeddings to understand the underlying emotion and context of a user's problem, rather than relying on basic keyword searches.
- **Zero-Hallucination Architecture:** The LLM generates answers *strictly* based on the retrieved public-domain verses, ensuring absolute scriptural accuracy and preventing AI hallucinations.
- **Built-in Crisis Gateway:** An intelligent intent-classifier that detects severe mental health distress (e.g., self-harm) and immediately pauses the spiritual guidance to provide verified national helpline numbers (Tele-MANAS).
- **Multi-lingual Output:** Capable of understanding and responding in English, Hindi, and Hinglish.

## 🛠️ Tech Stack

- **Backend:** Node.js, Express.js (or standard JS scripts for MVP)
- **AI & Embeddings:** Google Gemini API (`gemini-1.5-flash` for generation, `text-embedding-004` for vectors)
- **Database (MVP):** Local JSON / MongoDB Atlas Vector Search
- **Data Source:** Public domain Sanskrit text and open-source English translations of the Bhagavad Gita (701 verses).

## 📂 Project Structure

\`\`\`text
gita-mvp/
├── data/
│   ├── gita.json           # Cleaned DB of 700 verses & translations
│   └── embeddings.json     # Generated vector embeddings
├── .env                    # API keys (Not uploaded to GitHub)
├── build.js                # Script to clean and format raw scripture data
├── embed.js                # Script to convert text to vector embeddings
├── ask.js                  # Main RAG engine and CLI chat interface
├── package.json            # Node.js dependencies
└── README.md               # Project documentation
\`\`\`

## ⚙️ Installation & Setup

**1. Clone the repository:**
\`\`\`bash
git clone https://github.com/your-username/vedottam.git
cd vedottam
\`\`\`

**2. Install dependencies:**
\`\`\`bash
npm install
\`\`\`

**3. Configure Environment Variables:**
Create a `.env` file in the root directory and add your Google Gemini API key:
\`\`\`env
GEMINI_API_KEY=your_google_api_key_here
\`\`\`

**4. Build Data & Generate Embeddings:**
*(Note: If the `gita.json` and `embeddings.json` are already provided in the repo, you can skip this step.)*
\`\`\`bash
node build.js
node embed.js
\`\`\`

**5. Run the Application:**
\`\`\`bash
node ask.js
\`\`\`

## ⚠️ Disclaimer

Vedottam is an experimental AI project intended for spiritual guidance and educational purposes only. It is **not** a substitute for professional medical advice, diagnosis, or psychiatric therapy. If you are experiencing a mental health crisis, please reach out to a certified professional or call your national emergency helpline.

## 👨‍💻 Developed By

**Dev Rajpoot**  
B.Tech CSE | AI & Full-Stack Developer  
[LinkedIn](https://www.linkedin.com/in/dev-rajpoot-98086a320/) | [GitHub](https://github.com/devrajpoot2903-del)