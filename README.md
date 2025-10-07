## Caprae Capital Pre-Internship: AI-Powered Lead Generation Tool

<br>

This repository contains the code and documentation for the pre-internship task assignment as part of the Full Stack Developer interview process at Caprae Capital. The project's goal is to enhance a lead generation tool by integrating two key features that leverage AI to provide actionable insights for sales outreach.

-----

### 🚀 Features

This project implements two core features designed to improve the quality and relevance of leads.

1.  **Similar Companies Finder:** This feature identifies and provides a list of companies that are similar to a given company. It uses a similarity algorithm based on key attributes such as industry, company size, revenue, and technology stack to create a B2B "lookalike" audience.
2.  **Company Description & Goal Analyzer:** This feature scrapes public-facing content from a company's website and uses the Gemini API to analyze the text. It extracts a structured output in JSON format that includes the company's business summary, core mission, and key goals. This provides valuable context for sales teams.

-----

### 🛠️ Technologies Used

The solution is built using a modern AI-first tech stack.

  * **Python:** The core programming language for the back-end logic.
  * **Google Search API:** Used to programmatically search for relevant company websites.
  * **Gemini API:** The core AI model used for the "Company Description & Goal Analyzer" feature to process and extract structured data from unstructured text.
  * **`requests` & `BeautifulSoup`:** Libraries used for web scraping to retrieve content from websites.
  * **`pandas` & `scikit-learn`:** Used for data manipulation and to implement the similarity algorithm for the "Similar Companies" feature.

-----

### 📝 Solution and Approach

This project demonstrates a **"Quality First"** approach by focusing on providing **actionable insights** rather than just raw data. The solution is broken down into two primary components:

  * **Data Collection:** The tool uses a search API to find relevant company websites. It then scrapes public content from these sites, which is then stored in a temporary document.
  * **AI-Powered Analysis:** The combined scraped text is fed into the Gemini API with a detailed prompt. The API is instructed to return a structured JSON object, ensuring the output is clean and easy to use. This method is highly efficient and scalable, eliminating the need for complex, manual text parsing.

The implementation is a testament to the efficient use of modern tools to solve a real-world business problem within a tight time constraint.

-----

### ⚙️ Setup and Installation

Follow these steps to set up the project locally and run the code.

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/your-repository-name.git
    cd Caprae-Capital_PreInternship
    ```
2.  **Create a virtual environment:**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```
3.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
    (Note: You will need to create a `requirements.txt` file containing the project's dependencies, such as `requests`, `BeautifulSoup4`, `google-generativeai`, `pandas`, and `scikit-learn`.)
4.  **Configure API Keys:**
      * Obtain a **Google API Key** and a **Custom Search Engine ID (CSE ID)** and set them as environment variables.
      * Obtain your **Gemini API Key** and set it as an environment variable.
      * ```bash
          export GOOGLE_API_KEY="your_api_key"
          export GOOGLE_CSE_ID="your_cse_id"
          export GEMINI_API_KEY="your_gemini_api_key"
        ```
5.  **Run the script:**
    Run the Python notebook cell one by one.
