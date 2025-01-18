# AIscraper

AI scraper is a Streamlit-based web scraping application designed to simplify the process of extracting data from web pages. It allows users to specify URLs and data fields interactively, facilitating the extraction and manipulation of web data.

### Features

- Easy-to-use web interface.
- Custom field specification for data extraction.
- Pagination.
- Dynamic data processing with Python and Streamlit.
- Direct download capabilities for extracted data in various formats.
- Attended mode.
- AI-powered data extraction using models like OpenAI GPT, Google Gemini, and Llama.

### Prerequisites

Before you begin, ensure you have the following installed:
- Python 3.6 or higher
- Pip for managing Python packages

### Installation

Follow these steps to get your development environment running:

```bash
# Clone the repository
git clone https://github.com/redaelkate/AIscraper
cd scrape-master

# It's recommended to create a virtual environment
python -m venv venv
# Activate the virtual environment
# On Windows
venv\Scripts\activate
# On MacOS/Linux
source venv/bin/activate

# Install the required packages
pip install -r requirements.txt
```

### Launching the Application

To run AIscraper, navigate to the project directory and run the following command:

```bash
streamlit run streamlit_app.py
```

### Usage

After launching the application, open your web browser to the indicated address (typically `http://localhost:8501`). Use the sidebar to input the URL and fields you wish to scrape, then click the "Scrape" button to see results.

### How AI is Used

1. **Data Extraction**:
   * The application uses AI models (e.g., OpenAI GPT, Google Gemini, or Llama) to extract structured data from web pages.
   * You can specify the fields you want to extract (e.g., `name`, `price`, `description`), and the AI will automatically identify and extract these fields from the webpage content.

2. **Dynamic Schema Generation**:
   * Based on the fields you provide, the application dynamically generates a schema for the AI to follow.
   * This ensures the extracted data is structured and consistent.

3. **Data Formatting**:
   * The AI formats the extracted data into clean JSON and Excel files, making it easy to analyze or integrate with other tools.

4. **Handling Complex Content**:
   * The AI can handle missing or incomplete data, as well as content in foreign languages, ensuring robust extraction even from challenging web pages.

5. **Token Management**:
   * The application trims large web pages to fit within the AI model's token limits, ensuring efficient processing without losing critical data.

6. **Cost Calculation**:
   * The app calculates the cost of using the AI model based on the number of tokens processed, helping you manage your AI usage budget.

### Steps to Use

1. Enter the URL of the webpage you want to scrape.
2. Specify the fields you want to extract (e.g., `title`, `price`, `description`).
3. Select the AI model you want to use (e.g., OpenAI GPT, Google Gemini, or Llama).
4. Click "Scrape" to start the extraction process.
5. Download the extracted data in JSON or Excel format.

### Additional Notes

* **Attended Mode**: Use attended mode for interactive scraping, where you can manually guide the scraper through the process.
* **Pagination**: The scraper supports pagination, allowing you to scrape multiple pages of data seamlessly.
* **AI Model Selection**: Choose from supported AI models (OpenAI GPT, Google Gemini, or Llama) based on your requirements and budget.
* **Token Management**: The application automatically trims large web pages to fit within the AI model's token limits, ensuring efficient processing.
* **Cost Calculation**: The app calculates the cost of using the AI model based on the number of tokens processed, helping you manage your AI usage budget.
