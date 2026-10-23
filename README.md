# 🏗️ Construction Intelligence Platform

An AI-powered construction site assistant designed to support **site safety inspections, structural crack analysis, project cost estimation, and construction-related decision-making** using multimodal AI.

Built with Streamlit and Google Gemini as part of **Skill Wallet Capstone Project – 1**.

## 🚀 Key Features

### 1. 🦺 Safety & PPE Audit
- Analyze construction site photos using AI.
- Identify visible PPE items, including helmets, safety vests, boots, and safety harnesses.
- Highlight potential hazards with severity levels and suggested corrective actions.
- Generate a safety score from 0–100.
- Export the audit results as a downloadable JSON report.

### 2. 🧱 Crack Diagnostics
- Analyze uploaded wall and concrete images.
- Identify potential crack or defect types.
- Estimate crack width and assess apparent severity.
- Explore possible root causes, recommended repairs, and urgency levels.

*Note: AI-based visual assessments are preliminary and should be verified by a qualified structural engineer.*

### 3. 📊 Planning & Valuation
- Estimate project budgets and expenditure.
- Calculate approximate current asset value in INR.
- Estimate steel and cement requirements.
- Generate estimates based on structure type, construction area, location tier, and project completion percentage.

### 4. 🤖 AI Site Assistant
- Interact with an AI-powered construction engineering chatbot.
- Receive weather-aware safety guidance for wind, rain, and extreme heat.
- Ask construction-related questions through a multi-turn chat interface.

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Python 3.9+ | Core application logic |
| Streamlit | Interactive web interface |
| Google Gemini API | Multimodal AI analysis and responses |
| `google-genai` | Gemini API integration |
| `python-dotenv` | Environment variable management |
| JSON Schemas | Structured AI responses |

## ⚙️ Getting Started

### Prerequisites
- Python 3.9 or later
- A Google Gemini API key

### Installation

**1. Clone the repository**

```bash
git clone <repository-url>
cd <project-folder>
```

Replace the placeholders with your repository URL and project directory name.

**2. Create and activate a virtual environment (recommended)**

```bash
python -m venv .venv
```

Windows:

```bash
.venv\Scripts\activate
```

**3. Install dependencies**

```bash
pip install -r requirements.txt
```

**4. Configure your API key**

Get an API key from [Google AI Studio](https://aistudio.google.com/apikey).

Create a `.env` file in the project root:

```env
GEMINI_API_KEY=your_api_key_here
```

Replace `your_api_key_here` with your actual API key. Never commit your `.env` file or expose API credentials publicly.

Alternatively, use the API key input available in the application's sidebar, if configured.

**5. Launch the application**

```bash
streamlit run app.py
```

Open the local URL displayed in your terminal to access the application.

*Ensure that `requirements.txt`, `app.py`, and the referenced project files exist at the specified locations. Adjust the commands if your project structure differs.*

## 🖼️ Sample Images

The repository includes sample images for quick testing:

- `helmet.jpeg` — Safety and PPE audit
- `wall.jpeg` — Crack diagnostics

Upload these images in the relevant sections to explore the application's capabilities.

## ⚠️ Limitations & Considerations

- **Cost estimation:** Budget, asset valuation, and material quantities rely on approximate rates and assumptions. Actual costs vary by location, material prices, and project specifications.
- **Visual analysis:** Results depend on image quality, lighting, camera angle, and the information visible in the uploaded photo.
- **Structural assessment:** Crack analysis is intended for preliminary decision support, not as a replacement for an on-site inspection or professional structural evaluation.
- **AI reliability:** Outputs may contain inaccuracies and should be reviewed before making safety, engineering, or financial decisions.
- **API availability:** Gemini response times, usage limits, and temporary service errors may affect performance.

## 🔮 Project Objective

The goal of this project is to explore how multimodal AI can support construction workflows by combining image analysis, structured reporting, estimation tools, and conversational assistance in a single application.

---

**Project:** Construction Intelligence Platform  
**Category:** AI/ML · Generative AI · Multimodal Applications  
**Interface:** Streamlit  
**AI Integration:** Google Gemini
