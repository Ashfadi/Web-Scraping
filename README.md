# National Parks Data Extraction Project

## Overview
This project focuses on extracting and organizing data about U.S. National Parks from the [National Park Service website](https://www.nps.gov/index.htm). The data includes park names, categories, descriptions, addresses, phone numbers, and social media links, gathered programmatically using Python and web scraping techniques.

## Objectives
1. Extract links to all U.S. states from the National Park Service website.
2. Collect information about each park in every state, including:
   - Park Name
   - Category (e.g., National Monument, National Park, etc.)
   - Description
   - Address (split into multiple lines)
   - City, State, and Zip Code
   - Phone Number
   - Social Media Links (Facebook, Twitter, Instagram, YouTube, Flickr)
3. Store the extracted data in a CSV file with a standardized schema.

---

## Tools and Technologies
- **Programming Language**: Python
- **Libraries**:
  - `requests` for sending HTTP requests.
  - `BeautifulSoup` (from `bs4`) for web scraping.
  - `pandas` for data manipulation and storage.

---

## Steps

### **1. Retrieve Links to States**
- Scraped the main National Park Service website to extract links for all states using the dropdown menu.

### **2. Extract Park Data**
- For each state, navigated to its page to extract the list of parks, including:
  - Name, category, and description.
  - Links to individual park pages.

### **3. Extract Detailed Park Information**
- From each park’s page, extracted detailed information such as:
  - Address (Line 1, Line 2, Line 3).
  - City, state, and zip code.
  - Phone number and available social media links.

### **4. Store Data in CSV**
- All data was cleaned and stored in a CSV file (`All_Parks_Data.csv`) with the following columns:
  - Name
  - Category
  - Description
  - Street Address Line 1
  - Line 2
  - Line 3
  - City
  - State
  - Zip Code
  - Phone Number
  - Facebook
  - Twitter
  - Instagram
  - YouTube
  - Flickr

---

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/National-Parks-Data-Extraction.git
