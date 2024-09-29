
# AI Web Scraper using Python and Ollama

This project is an AI-powered web scraping tool built with Python, integrating Ollama's LLM for language processing and Streamlit for an interactive UI. The scraper leverages ChromeDriver for web automation and scraping.

## Prerequisites

Before running the project, ensure that you have installed the following tools:

1. **Python** (version 3.7+ recommended)
2. **ChromeDriver** for web scraping
3. **Ollama** for AI language model processing
4. **Streamlit** for building the user interface

## Installation Guide

### Step 1: Install ChromeDriver

ChromeDriver is used to automate tasks in Google Chrome for scraping purposes. You can download the latest version of ChromeDriver from the link below:

[Download ChromeDriver](https://googlechromelabs.github.io/chrome-for-testing/#stable)

- Once downloaded:
  1. Unzip the file.
  2. Move the `chromedriver` file to a folder where it can be easily accessed.
  3. Update the path in the `scrape.py` file:

    ```python
    from selenium import webdriver

    # Replace with the path to your downloaded chromedriver
    driver = webdriver.Chrome(executable_path='/path/to/chromedriver')
    ```

### Step 2: Install Ollama

Ollama provides the large language model (LLM) that powers the AI capabilities of this project. Download and install Ollama from the link below:

[Download Ollama](https://ollama.com/)

- After installation, pull the required LLM model by running:

    ```bash
    ollama pull llama3.1
    ```

- Once the model is downloaded, start the LLM with:

    ```bash
    ollama run llama3
    ```

### Step 3: Install Project Dependencies

Make sure you have the required Python libraries installed. You can install them using `pip`:

```bash
pip install -r requirements.txt
```

### Step 4: Running the Application

To run the web scraper and interact with the AI model, follow these steps:

1. **Start the Ollama server**  
   Make sure Ollama is running the required LLM by executing the command:
   
   ```bash
   ollama run llama3


2. **Run the Streamlit app**  
   In another terminal window, navigate to the project directory and launch the Streamlit app by executing the following command:

   ```bash
   streamlit run main.py
