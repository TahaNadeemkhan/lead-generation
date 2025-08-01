# 🚀 Lead Scraper Pro: AI-Powered Lead Generation Tool

## ✨ Project Overview

Lead Scraper Pro is a powerful, open-source Streamlit application designed to automate the process of lead generation. It uses a combination of intelligent AI agents, web scraping, and API integrations to find and extract valuable contact and company information.

This tool is built to solve the common problem of manually searching for leads across multiple platforms, saving you significant time and effort. It provides two core functionalities:

1.  **👤 Lead Contacts Scraper:** Find emails, phone numbers, names, and company details for individuals across popular professional and social platforms like LinkedIn, GitHub, and more.
2.  **💰 Company Funding Scraper:** Discover recently funded companies in a specific industry and enrich their profiles with detailed information from sources like Apollo.io.

The application is built with a focus on simplicity, featuring a user-friendly interface powered by Streamlit that makes the complex process of web scraping accessible to everyone.

## 🛠️ Features

* **AI-Powered Search:** Uses an AI agent to intelligently formulate search queries and find relevant URLs from various social and professional networks.
* **Multi-Platform Scraping:** Scrapes data from multiple websites including `linkedin.com`, `github.com`, `facebook.com`, and `twitter.com` for individual leads.
* **Targeted Funding Search:** Scrapes recent funding news from sites like `crunchbase.com`, `techcrunch.com`, and `venturebeat.com`.
* **Intelligent Data Extraction:** Extracts emails, phone numbers, names, and company details from unstructured website content.
* **Apollo.io Integration:** (Optional) Enriches company funding data with comprehensive details such as CEO name, company phone, employee count, and revenue using the Apollo.io API.
* **Data Persistence:** Uses `st.session_state` to prevent the app from restarting and losing data on every user interaction.
* **Downloadable Results:** Export your scraped leads and company data directly as a CSV file.

## ⚙️ Installation and Setup

### Prerequisites

* Python 3.8+
* Git

### Steps

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/your-username/lead-scraper-pro.git](https://github.com/your-username/lead-scraper-pro.git)
    cd lead-scraper-pro
    ```

2.  **Create a virtual environment (recommended):**
    ```bash
    python -m venv venv
    source venv/Scripts/activate  # On Windows
    source venv/bin/activate      # On macOS/Linux
    ```

3.  **Install the required dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
    _Note: The `requirements.txt` file should contain all the necessary libraries like `streamlit`, `requests`, `pandas`, `beautifulsoup4`, `langchain`, `python-dotenv`, etc._

4.  **Set up API Keys:**
    This application uses several APIs for its core functionality. You need to create a `.env` file in the project's root directory and add your API keys there.

    * **Serper API Key:** For Google Search. [Get it here](https://serper.dev/).
    * **Gemini API Key:** For the AI agent. [Get it here](https://aistudio.google.com/app/apikey).
    * **Apollo.io API Key (Optional):** For company data enrichment. [Get it here](https://www.apollo.io/).

    Your `.env` file should look like this:
    ```
    SERPER_API_KEY="your_serper_api_key_here"
    GEMINI_API_KEY="your_gemini_api_key_here"
    APOLLO_API_KEY="your_apollo_api_key_here"
    ```

## ▶️ How to Run the App

Run the Streamlit application with:
```bash
streamlit run app.py
```

Replace `app.py` with the actual name of your Python script (e.g., `main.py`).

The application will open in your web browser. If it doesn't, copy the provided local URL (e.g., `http://localhost:5000`) and paste it into your browser's address bar.

## 🚀 How to Use the App

### 👤 Lead Contacts

1. Navigate to the **Lead Contacts** tab.
2. Enter the `Job Title` and `Location` of the leads you are looking for.
3. Click the **🔎 Start Lead Contact Scraping** button. The app will search for relevant public profiles and extract contact details.
4. Once the process is complete, results will be displayed in a table. Use the radio buttons to filter results (e.g., *Email Only*, *Both Email & Phone*).
5. Click the **Download** button to save the filtered data.

### 💰 Company Funding

1. Navigate to the **Company Funding** tab.
2. Enter `Keywords` for the industry you're interested in (e.g., *AI*, *Fintech*).
3. Select a **Funding Activity After Date** to find recent funding rounds.
4. Click the **🔎 Start Company Funding Scraping** button. The app will search for articles and press releases about company funding.
5. Results will be displayed in a table. If an Apollo.io API key is provided, the data will be enriched with additional company and CEO details.
6. Click the **Download** button to save the complete dataset.

## 🤝 Contributing

Contributions make the open-source community an amazing place to learn, inspire, and create. Any contributions are **greatly appreciated**!

1. Fork the Project.
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`).
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`).
4. Push to the Branch (`git push origin feature/AmazingFeature`).
5. Open a Pull Request.

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.

---

*Project made with ❤️ by **Taha Nadeem Khan***
```
