# 🚀 AI Versus Automation Workflow

An end-to-end AI-powered automation system that generates viral "versus" videos (e.g., Lion vs Tiger) including scenes, images, and final rendered videos — and automatically publishes them to social media.

---

## 📌 Overview

This project is built using **n8n** and integrates multiple AI + media APIs to fully automate content creation:

- Generates battle matchups
- Creates cinematic AI images
- Produces final videos
- Publishes to Instagram, TikTok, and YouTube

---

## ⚙️ Workflow Breakdown

### 1. 🎬 Create Scenes
- Fetches a main character from Google Sheets  
- Uses AI to generate 8 opponents  
- Structures data into scenes  

### 2. 🖼️ Create Close-up Images
- Generates high-quality AI prompts  
- Calls image generation API  
- Stores generated images  

### 3. 🏆 Create Winner Images
- Creates cinematic "battle result" images  
- Determines winner realistically  
- Generates final scene visuals  

### 4. 🎥 Render Video
- Uses Creatomate API to render final video  
- Combines all generated assets  
- Outputs a ready-to-publish video  

### 5. 📤 Auto Publishing
- Uploads video via Blotato  
- Publishes to:
  - Instagram  
  - TikTok  
  - YouTube  

---

## 🧠 Tech Stack

- **n8n** – workflow automation  
- **OpenRouter (GPT-4.1 / GPT-4.1-mini)** – AI generation  
- **PiAPI (Flux model)** – image generation  
- **Creatomate** – video rendering  
- **Google Sheets** – data storage  
- **Blotato API** – social media publishing  

---

## 🔧 Setup Instructions

1. Clone this repository  
2. Import the workflow (`AI_Versus.json`) into n8n  
3. Configure the following APIs:
   - OpenRouter API key  
   - PiAPI key  
   - Creatomate template + API key  
   - Google Sheets connection  
   - Blotato API key  

4. Update placeholders in the workflow:
   - `YOUR API KEY`
   - `YOUR TEMPLATE ID`
   - `account_id`

5. Run the workflow or schedule it using the trigger  

---

## 📊 Data Flow

Google Sheets → Scene Generation → Image Generation → Video Rendering → Upload → Social Media

---

## 📁 Files

- `AI_Versus.json` → Main n8n workflow  
- `workflow1 ss.png` → Visual workflow diagram  

---

## 🚀 Features

- Fully automated content creation  
- AI-generated battle scenarios  
- High-quality cinematic images  
- Auto video rendering  
- Multi-platform publishing  

---

## ⚠️ Notes

- Requires API credits for external services  
- Image/video generation may take time (~90 seconds delays configured)  
- Ensure proper API limits and quotas  

---

## 👤 Author

**Bunny Tripathi**

---

## ⭐ Future Improvements

- Add more content formats  
- Improve prompt quality  
- Add analytics tracking  
- Support more social platforms  

---

## 📌 Example Use Case

Generate viral short videos like:

> "Lion vs Tiger – Who Wins?"

Automatically created and posted without manual work.

---

## 🧩 Workflow Preview

![Workflow](workflow1%20ss.png)

---
