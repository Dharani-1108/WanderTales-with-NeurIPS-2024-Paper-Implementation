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
- Led project coordination to ensure all team deliverables were met on time.
- Designed and implemented **Amadeus API integration**, transforming raw flight data into structured formats.
- Unified APIs (**Amadeus**, **Google Maps**, **OpenWeather**) for end-to-end itinerary generation.
- Converted API responses into **vector embeddings** for use in the **RAG-based pipeline**.
- Developed an **interactive chatbot interface** to gather user preferences and refine trip plans.
- Compared **Stable Diffusion vs. DALL·E** for generating AI-based visuals and video previews.
- Built visualizations including **RAG attention heatmaps** and **interactive Folium maps**.
- Implemented **DiffCut segmentation** to isolate subjects and blur backgrounds in generated images.


**🔧 Skillset:**  
Python, Streamlit, React.js, REST APIs, Machine Learning, Deep Learning, Data Science

---

### 🚀 Dharani Thakkallapally (AI & NLP Engineer)
- Generated **AI travel stories, visuals, and video outputs** for personalized trip summaries.
- Experimented with **LLaMA**, **Mistral 7B**, and other open-source LLMs to reduce reliance on OpenAI.
- Attempted realistic video generation; pivoted to optimized zoom/pan animations due to model access limitations.
- Enhanced **prompt engineering** to improve relevance and narrative coherence.
- Integrated **purpose of visit** into story generation for higher personalization.
- Investigated **LoRA fine-tuning** for GPT-4, confirmed weight restrictions prevent it.
- Deployed the complete application on **Streamlit**.
- Created the **demo video** and **poster** for the Research-A-Thon.
- Authored **Progress Report 2** and handled **LLM-Check paper reproduction** with metric analysis and documentation.
**🔧 Skillset:**  
Python, NLP, Hugging Face Transformers, GPT models, Machine Learning, Deep Learning, Data Science, Cloud Platforms

---

### 🔗 Pavan Sundar Reddy Guthikonda (Backend & API Integration)
- Developed the **Frontend using Streamlit**, building responsive and user-friendly UI components.
- Resolved **deployment issues**, including **MoviePy** failures that occurred only on Streamlit Cloud.
- Integrated APIs and ensured smooth data flow and **real-time UI rendering**.
- Enhanced **application performance** using **asynchronous API calls** and layout optimization.
- Worked on **RAG (Retrieval-Augmented Generation)**:
  - Set up document embedding and vector indexing.
  - Implemented **reranking strategies** to improve relevance.
  - Compared **hallucination rates in RAG vs non-RAG** pipelines to improve story reliability.

**🔧 Skillset:**  
Python, Flask, FastAPI, Node.js, SQL Databases, REST APIs, Data Science, Machine Learning, Deep Learning

---

### 🎯 Banu Teja Jampani (Tester)
- Designed and implemented the **personalized recommendation engine** using user preferences and rule-based filters.
- Enabled dynamic updates based on **real-time inputs** like weather and transport delays.
- Conducted **story coherence validation** and assisted in documentation of the reproducibility process and workflow.

**🔧 Skillset:**  
Python, Machine Learning, Data Science

---
## 📌 **YouTube Link**
### https://www.youtube.com/watch?v=KmgBMrlUTYE
---
## 🔧 **Troubleshooting**
### ⚠️ **Common Issues & Fixes**:
- **❌ Invalid API Key Error?** → Ensure your **API keys** are **correctly set**.  
- **📦 Module Not Found Error?** → Run `pip install -r requirements.txt` again.  
- **🚀 Streamlit App Not Running?** → Make sure to **activate the virtual environment** before running the app.  

---

📌 **Developed by:** [The WanderCoders Team] 🚀🎉  
🎓 **Powered by** NeurIPS 2024 open-source research for real-world AI applications.

