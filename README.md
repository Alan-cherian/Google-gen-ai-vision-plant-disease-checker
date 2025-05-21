# Google-gen-ai-vision-plant-disease-checker
🌱 Project Report: Multi-Language Plant Disease Detection using Gemini AI

🔍 Project Title

Intelligent Multi-Lingual Plant Disease Analyzer using Gemini AI

📌 Objective

To automatically detect plant diseases from images using Google's Gemini AI and generate detailed diagnostic reports in multiple languages (English, Hindi, Japanese, French).

🧠 Key Features

Accepts folder of plant images for batch processing.

Uses Gemini 2.0 Flash via LangChain to analyze each image.

Multilingual output support:

English

Hindi

Japanese

French

Each output file contains:

Timestamp

Image name

Diagnosis (disease name, symptoms, and treatment)

Saves results in separate text files named per language and date.

Uses multithreading for efficient image analysis.

🛠️ Tech Stack

Language: Python

Libraries Used: os, base64, time, threading, langchain-google-genai

AI Model: Gemini AI (via ChatGoogleGenerativeAI)

📂 Project Structure

plant-disease-analyzer/
️️️️️
├── images/                                  # Folder containing input plant images
├── plant_disease_observations_en_YYYY-MM-DD.txt
├── plant_disease_observations_hi_YYYY-MM-DD.txt
├── plant_disease_observations_ja_YYYY-MM-DD.txt
├── plant_disease_observations_fr_YYYY-MM-DD.txt
├── plant_disease_analyzer.py               # Main script

📚 Gemini Prompt Template

You are an expert agricultural assistant. 
Analyze the image of this plant and provide the following in [LANGUAGE]:
1. Name of the disease (if any)
2. Description of symptoms
3. Suggested treatment or medicine

🖋️ Sample Output (English)

2025-05-21 15:34:10 | leaf_blight_01.jpg | 
• Disease: Leaf Blight
• Symptoms: Yellowing and browning of leaf edges.
• Treatment: Apply copper-based fungicide; remove infected leaves.

🌟 Applications

Agricultural monitoring

Smart farming and precision agriculture

Rural farmer assistance via mobile apps

✅ Future Improvements

Add support for audio alerts in local languages.

Integrate with drone/robot platforms for autonomous scanning.

Build GUI-based system for ease of use by farmers.
