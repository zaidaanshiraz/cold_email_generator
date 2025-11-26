# 📧 Cold Email Generator

## Project Overview
The Cold Email Generator is a sophisticated, AI-powered tool designed to streamline the outreach process for services companies. It leverages the power of the Groq API for rapid large language model (LLM) inference, LangChain for complex prompt orchestration, and Streamlit for an interactive user interface.

The core function is to generate highly personalized and compelling cold emails by integrating three key data sources:
- **Job Market Demand:** Extracts live, specific job listings from a target company's careers page URL.
- **Portfolio Matching (Vector DB):** Queries an internal vector database (part of the backend architecture) to find the most relevant project examples or case studies that align with the skills required in the job description.
- **Personalized Outreach:** Uses the gathered data and portfolio matches to craft a targeted cold email, positioning the service provider’s dedicated resource as a superior, faster alternative to the standard hiring process.

## 🎯 The Scenario: Why This Tool Matters
Imagine:
- **The Target:** Nike is currently investing significant time and resources in recruitment, onboarding, and training for a role like Principal Software Engineer.
- **The Solution:** Atliq, a software development company, has a highly skilled engineer ready to deploy immediately.
- **The Outreach:** The Business Development Executive (Mohan) from Atliq uses this Cold Email Generator to reach out to Nike. The generated email addresses Nike’s specific pain points and offers a tailored solution with relevant portfolio proofs aligned with the job requirements, bypassing the slow hiring cycle.

## 🏗️ Architecture Diagram
The system operates on a layered architecture combining:
- Web scraping for live job listings
- Vector search for portfolio matching
- Large language model for personalized email generation

## 🚀 Setup and Installation

### 1. Obtain Your Groq API Key
This application depends on the Groq API for fast email generation.

- Go to [Groq Console](https://console.groq.com/keys)
- Generate a new API Key.
- Update `.env` file in the `app/` directory:

