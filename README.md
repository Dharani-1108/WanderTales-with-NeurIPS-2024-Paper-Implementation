# 🌍✈️ **WanderTales AI Travel Planner**
🚀 **Your AI-powered assistant for effortless travel planning!**  

WanderTales AI creates **personalized travel plans** with **immersive AI-generated stories, real-time flight & hotel details, weather forecasts, hallucination-checked storytelling, and stunning AI-generated images & videos.**  

---

## 📌 **Key Features**
**📑 Smart Itinerary** – Personalized accommodations, attractions & dining recommendations  
**🛴 AI Travel Story** – Engaging, narrated travel experiences  
**🎤 AI Voiceover** – Listen to your travel story  
**🖼️ AI-Generated Images** – Unique visuals for your journey  
**🎥 AI-Powered Travel Video** – Cinematic trip montages  
**🌦 Live Weather Updates** – Stay prepared  
**🏨 Hotel & 🍽️ Restaurant Suggestions** – Top-rated places to stay & dine  
**✈️ Real-Time Flights** – Up-to-date flight details  
**🧠 Hallucination Detection** – Reliable and validated travel storytelling using LLM-Check  
**🎨 Image Segmentation** – Subject-background separation via DiffCut  

---

## 🧠 **Research-Driven Enhancements (NeurIPS 2024 Paper Integration)**

### 📄 **Paper 1: DiffCut – Zero-Shot Image Segmentation**
- Integrated **DiffCut** to auto-detect and segment landmarks, people, and objects in user-uploaded or AI-generated photos.  
- Used **Latent Diffusion Model (LDM)** and **Recursive Normalized Cut** to create zero-shot segmentation masks.  
- Applied **PAMR** and **median filtering** for post-processing.  
- Generated **overlay** and **blurred background isolation views** to enhance story visuals.  
- Reproduced core visuals from the paper and demonstrated with custom travel photos in the app.  

> 📸 *“Auto-segment and spotlight your memories.”*

---

### 📄 **Paper 2: LLM-Check – Hallucination Detection for Narratives**
- Integrated **LLM-Check** to evaluate AI-generated travel stories for hallucinations.  
- Ran evaluation using **GPT-2, GPT-Neo-1.3B**, and **LLaMA-2-7B**.  
- Computed **perplexity** and **entropy** scores for both **RAG** and **non-RAG** outputs.  
- Handled Hugging Face model loading, token setup, and quantized model optimization.  
- Filtered or flagged hallucinated responses to improve user trust in storytelling.  

> 🧾 *“Travel stories you can trust – evaluated for factual accuracy.”*


---

## 🛠 **Setup & Installation**
### 📌 **1. Clone the Repository**
```bash
git clone https://github.com/pavan7357/WanderTales-with-NeurIPS-2024-Paper-Implementation.git
cd WanderTales-with-NeurIPS-2024-Paper-Implementation
```
### 📌 **2. Create a Virtual Environment**
```bash
python -m venv wander_env
source wander_env/bin/activate   # For macOS/Linux
wander_env\Scripts\activate      # For Windows**
```
### 📌 **3. Install Dependencies**
```bash
pip install -r requirements.txt
```

### 📌 **4. Set API Keys (Environment Variables)**
You must set the following API keys before running the project:
```bash
export OPENAI_API_KEY="your-openai-api-key"
export GOOGLE_MAPS_API_KEY="your-google-maps-api-key"
export WEATHER_API_KEY="your-weather-api-key"
export AMADEUS_API_KEY="your-amadeus-api-key"
export AMADEUS_API_SECRET="your-amadeus-api-secret"
```
Alternatively, you can store them in **secrets.toml** for Streamlit deployment.

---


## 👥 **Team Name: The WanderCoders**

---

### 🎨 Viswanth Tammana (Frontend Developer | Team Lead)
- Reproduced and enhanced **DiffCut** integration into the frontend.
- Used AI-generated travel images to apply zero-shot segmentation and background blurring.
- Built the UI using **Streamlit** to showcase masked visuals and support dynamic story visuals.
- Currently working on full integration of **DiffCut** into the WanderTales storytelling pipeline.

**🔧 Skillset:**  
Python, Streamlit, React.js, REST APIs, Machine Learning, Deep Learning, Data Science

---

### 🚀 Dharani Thakkallapally (AI & NLP Engineer)
- Integrated the **LLM-Check** hallucination evaluation method into the WanderTales project.
- Evaluated hallucination risks using **perplexity and entropy** metrics across **GPT-2, GPT-Neo-1.3B, and LLaMA-2-7B**.
- Handled Hugging Face model setup, authentication, and dependency installation.
- Summarized findings in a reproducibility report with detailed metric insights.

**🔧 Skillset:**  
Python, NLP, Hugging Face Transformers, GPT models, Machine Learning, Deep Learning, Data Science, Cloud Platforms

---

### 🔗 Pavan Sundar Reddy Guthikonda (Backend & API Integration)
- Developed and maintained the **Flask/FastAPI** backend architecture.
- Integrated real-time APIs: **Google Maps, Amadeus, OpenWeather, SerpAPI** for dynamic data fetching.
- Managed local storage and backend-to-frontend communication.
- Partially contributed to the **hallucination rate evaluation** by comparing **RAG vs non-RAG** narrative outputs.

**🔧 Skillset:**  
Python, Flask, FastAPI, Node.js, SQL Databases, REST APIs, Data Science, Machine Learning, Deep Learning

---

### 🎯 Banu Teja Jampani (Tester)
- Designed and implemented the **personalized recommendation engine** using user preferences and rule-based filters.
- Enabled dynamic updates based on **real-time inputs** like weather and transport delays.
- Conducted **story coherence validation** and assisted in documentation of the reproducibility process and workflow.

**🔧 Skillset:**  
Python, Machine Learning, Deep Learning, Data Science, Recommender Systems, Blockchain Technologies

---

## 🔧 **Troubleshooting**
### ⚠️ **Common Issues & Fixes**:
- **❌ Invalid API Key Error?** → Ensure your **API keys** are **correctly set**.  
- **📦 Module Not Found Error?** → Run `pip install -r requirements.txt` again.  
- **🚀 Streamlit App Not Running?** → Make sure to **activate the virtual environment** before running the app.  

---

📌 **Developed by:** [The WanderCoders Team] 🚀🎉  
🎓 **Powered by** NeurIPS 2024 open-source research for real-world AI applications.

