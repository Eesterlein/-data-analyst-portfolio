# -data-analyst-portfolio
Interactive portfolio highlighting data projects, certifications, and skills

# Elissa Esterlein – Data Analyst Portfolio

## About

Hi, I'm Elissa. I bring a background in biology and medical research to the field of data analytics, with a strong interest in applying data-driven insights to health, environment, and public policy challenges.

After stepping away from research to raise my children and live off-grid in the Colorado Rockies, I’ve reignited my technical skills through modern tools like Python, geospatial analysis, and AI-assisted workflows. My passion for learning, curiosity about complex systems, and drive to uncover meaningful patterns have made data science an exciting new chapter in my career.

This portfolio showcases my work across a variety of domains — from exploring land ownership trends in Colorado, to building lightweight AI tools, to tracking real-time flight data near Gunnison Airport. These projects reflect my growing expertise in data wrangling, visualization, and storytelling through code.

I'm actively building my skills through certifications, real-world projects, and public data challenges — and I’m excited to contribute to mission-driven organizations as a flexible, creative, and thoughtful data analyst.

---

📍 Based in Colorado  

📁 View my resume [here](CV_pdf.pdf)  
📊 [Kaggle](https://www.kaggle.com/elissaesterlein) • [Tableau Public](https://public.tableau.com/app/profile/elissa.esterlein/vizzes) • [GitHub Projects](https://github.com/Eesterlein)

---

## 📑 Table of Contents

- [About](#about) 

### Portfolio Projects

#### Python  
- [Garmin Fitness Data Analysis](#garmin-fitness-data-analysis)
- [Colorado Land Ownership](#colorado-land-ownership)
- [Building Local Language Models](#building-local-language-models)  

#### Workplace Automation & Tools
- [MLS Photo Processor](#mls-photo-processor)
- [Gunnison County Property Analysis Map](#gunnison-county-property-analysis-map)
- [Zillow Property & Photo Scraper](#zillow-property-scraper-scraperapi-version)
  
  
#### SQL  
- [US State-level Demographics Snapshot](#US-State-level-Demographics-Snapshot)
  
#### R  
- *Coming Soon*

#### Web Development
- [Gunnison Airport Flight Tracker Website](#gunnison-airport-flight-tracker-website)
- [Gunnison County Housing Dashboard (Pre/Post COVID)](#gunnison-county-housing-dashboard-prepost-covid)
- [Residential Structure Conditions in Gunnison County](#residential-structure-conditions-in-gunnison-county)
 

#### Tableau  
- [My Tableau Public Profile](https://public.tableau.com/app/profile/elissa.esterlein)  

---

- [Education](#education)  

---

- [Certificates](#certificates)  

---

- [Contact](#contact)    


## Portfolio Projects  
In this section, I list data analytics and AI projects with brief summaries and links to source code or hosted reports.

---

### Garmin Fitness Data Analysis  
**Code:** [Garmin Fitness Analysis Repository](https://github.com/Eesterlein/My-2024-Garmin-Data-Analysis-)  
**Live Report:** [GitHub Pages Site](https://eesterlein.github.io/My-2024-Garmin-Data-Analysis-/)

**Goal:** To uncover patterns in personal health data using Garmin fitness exports.

**Description:** This project explores trends in activity, calories, heart rate, sleep, and stress over the course of 2024. Using Python, I analyzed and visualized seasonality, correlations, and wellness insights from raw Garmin data.

**Skills:** data wrangling, time series analysis, statistical correlation, data storytelling.  
**Technology:** Python, Pandas, Matplotlib, Seaborn.

**Results:** Revealed a strong correlation between activity and calorie burn (0.89), seasonal changes in workout intensity, and a moderate link between resting heart rate and stress.

---

### Building Local Language Models  
**Code:** [Local LLM Chatbot Repo](https://github.com/Eesterlein/Building-Local-LLMs-for-Private-Workflows)

**Goal:** To create a privacy-first AI assistant using locally hosted large language models (LLMs).

**Description:** Built a demo app using Ollama, LlamaIndex, and LangChain that simulates a policy chatbot trained on company handbooks. The agent can answer questions locally without needing an internet connection.

**Skills:** vector database indexing, prompt engineering, RAG pipelines, local AI hosting.  
**Technology:** Python, Ollama, LangChain, LlamaIndex, Markdown, FastAPI (planned).

**Results:** Demonstrated how companies can use on-device models for internal knowledge queries without sharing data externally.

---

### MLS Photo Processor

**Code:** [MLS Photo Renaming & Classification Repo](https://github.com/Eesterlein/MLS-Photo-Processor)  

**Goal:** To automate the tedious process of renaming, sorting, and classifying MLS property photos for assessor and appraisal workflows.  

**Description:** Built a local desktop utility that uses AI to organize property images. The app matches user-provided parcel numbers to internal account records and uses a vision-language model (CLIP) to automatically "see" and label photos (e.g., Kitchen, Exterior, Bathroom). It transforms messy, randomly named downloads into standardized, system-ready files without any manual data entry.  

**Skills:** Zero-shot image classification, desktop GUI development, asynchronous processing, file system automation, data mapping.  

**Technology:** Python, PyTorch, Hugging Face (CLIP), Pandas, Tkinter, Pillow.  

**Results:** Eliminate manual renaming for high-volume photo sets. The tool provides deterministic, conservative classification—defaulting to "Other" if confidence is low—ensuring 100% reliable file naming and immediate compatibility with local government recording systems.

---

### Gunnison County Property Analysis Map
**Code:** [Gunnison GIS Mapping Static Demo](https://github.com/Eesterlein/gunnison_gis_mapping_static_demo)  
**Live Report:** [GitHub Pages Site](https://eesterlein.github.io/gunnison_gis_mapping_static_demo/html_map/)

**Goal:** To provide appraisers and GIS analysts with an interactive tool for visualizing property attributes and identifying data discrepancies across Gunnison County.

**Description:** Developed a lightweight, high-performance web mapping application that joins disparate assessment CSVs with GeoJSON parcel boundaries. The tool allows users to dynamically style parcels based on appraisal-critical features like quality, view descriptions, and total value. By isolating parcels with missing or outlier data, the application serves as a front-end interface for spatial data auditing and valuation analysis.

**Skills:** Geospatial data joining, thematic mapping, front-end web development, data integrity/QA.

**Technology:** JavaScript (ES6+), Leaflet.js, HTML5/CSS3, GeoJSON, CSV.

**Results:** Achieved a 97% data coverage rate by merging multiple assessment sources, enabling a "clean interface" approach where analysts can instantly identify and correct data gaps in the county's primary property records.

---

### Zillow Property & Photo Scraper [In Development]
**Code:** [Zillow Photo Scraper Repo](https://github.com/Eesterlein/zillow-photo-scraper-scraperapi)

**Goal:** To automate the extraction of property metadata and high-resolution images from Zillow for real estate appraisal and market analysis.

**Description:** Developed a Python-based scraping utility designed to bypass bot detection using ScraperAPI to retrieve listing data and image assets. The tool performs fuzzy address matching against a local CSV database to automatically organize downloads into account-specific directories. **Note:** This project is currently being refactored; an updated version utilizing Playwright and Chromium for enhanced browser automation and stability will be pushed soon.

**Skills:** Web scraping architecture, API integration (ScraperAPI), data normalization, folder-structure automation, asynchronous asset downloading.

**Technology:** Python, Requests, Pandas, JSON, BeautifulSoup4 (Playwright/Chromium implementation pending).

**Results:** Built a functional pipeline that handles batch URL processing and auto-classifies images based on metadata hints, significantly reducing the manual effort required to compile subject property photo boards.

---

### Colorado Land Ownership   
**Code:** [Colorado Land Ownership GitHub Repo](https://github.com/Eesterlein/colorado-land-ownership)  
**Live Report:** [GitHub Pages Site](https://eesterlein.github.io/colorado-land-ownership/)

**Goal:** To analyze the distribution of public vs. private land ownership across Colorado and explore trends in absentee ownership.

**Description:** This geospatial project combines COMaP shapefiles, parcel data, and assessor records to visualize land control by agency, ownership type, and residency.

**Skills:** geospatial analysis, public land data, mapping, data cleaning, visualization, storytelling.  
**Technology:** Python, GeoPandas, Matplotlib, ArcGIS, GitHub Pages.

**Results:** Found that 62.6% of Colorado is privately owned; in counties like Gunnison, over 76% is public land, but private parcels are increasingly owned by out-of-county residents and investment entities.

---

### US State-level Demographics Snapshot
**Code:** [US State-level Demographics Snapshot Repo](https://github.com/Eesterlein/us-state-demographics-sql-acs2019)  
**Live Report:** [Looker Studio](https://lookerstudio.google.com/s/mNjbN_gsXoQ)

**Goal:**  
To analyze state-level socioeconomic indicators using U.S. Census ACS data and uncover patterns in poverty, income, education, housing, and inequality.

**Description:**  
This project uses SQL to process 2019 ACS data, calculate key metrics (poverty rate, income, unemployment, etc.), and rank states using window functions and case logic. The final dataset is visualized in Looker Studio with interactive maps and scorecards.

**Skills:**  
SQL joins, CTEs, window functions, CASE statements, aggregate functions, data type conversion, public data querying, dashboard design.

**Technology:**  
BigQuery, Looker Studio, GitHub, Google Cloud Console.

**Results:**  
Created a full-featured dashboard showing disparities in income, education, rent burden, and inequality across all U.S. states. Used SQL logic to categorize poverty levels, rank states, and feed geospatial visualizations.  

---

### Gunnison Airport Flight Tracker Website
**Code:** [Gunnison Airport Tracker GitHub Repo](https://github.com/Eesterlein/gunnison-airport-tracker)  
**Live Report:** [Heroku App](https://gunnison-airport-tracker-28d8dfff50df.herokuapp.com)

**Goal:** To build a real-time flight tracking system for private flights near Gunnison, CO, leveraging the OpenSky Network API and PostgreSQL for data storage.

**Description:** This web application tracks the location, altitude, and status of aircraft flying near Gunnison Airport (KGUC). The project integrates OpenSky API for real-time flight data, stores flight information in a PostgreSQL database, and displays the data on an interactive, user-friendly interface. Private plane logs are stored and queried based on repeat sightings.

**Skills:** API integration, web development, database management, real-time data processing, interactive visualization.  
**Technology:** Node.js, Express.js, OpenSky Network API, PostgreSQL, Heroku, HTML, CSS, JavaScript.

**Results:** Successfully built and deployed a functional flight tracker displaying real-time flights, with the ability to track and log private aircraft that fly over Gunnison regularly. The system fetches and updates flight data every hour, ensuring the live dashboard remains current.

---

## Gunnison County Housing Dashboard (Pre/Post COVID)

**Code:** [GitHub Repo](https://github.com/Eesterlein/gunnison-housing-snapshots)  
**Live Site:** [GitHub Pages](https://eesterlein.github.io/gunnison-housing-snapshots/)

**Goal:**  
Create an interactive, public-facing dashboard to compare **pre-COVID (2017–2018)** vs **post-COVID (2022–2023)** housing market conditions in Gunnison County, CO, and communicate affordability changes.

**Description:**  
Single-page web app with an **All property types** view and a **Residential proxy (≥800 sq ft)** lens. The app shows “typical sale” medians, price per sq ft, sales counts, quarterly medians/volume (with a dashed pre/post divider), a **Gunnison vs U.S.** context chart, and an **affordability** indicator (share of U.S. households able to afford, assuming 20% down, 30% payment-to-income, prevailing mortgage rates, and national median income).

**Skills:**  
Web development, data visualization, data cleaning, UX copy & layout, deployment (GitHub Pages)

**Results:**  
- **All property types (≤$15M):** median rose from **$305k** (2017–2018) to **$575k** (2022–2023); affordability fell from **42%** to **14%** of U.S. households.  
- **Residential proxy (≥800 sq ft):** median moved from **$343k** to **$650k** over the same periods.  
  
---

## Residential Structure Conditions in Gunnison County

**Code:** [GitHub Repo](https://github.com/Eesterlein/gunnison-residential-condition)  
**Live Site:** [GitHub Pages](https://eesterlein.github.io/gunnison-residential-condition/)

**Goal:**  
Develop two connected, interactive dashboards to visualize the **assessed condition and value of residential structures across Gunnison County, CO** — one focused on **primary improvements** (main dwellings) and another that includes **all residential improvements** throughout the valley.

**Description:**  
Built with **HTML, CSS, JavaScript, Plotly.js,** and **PapaParse**, these dashboards provide a transparent look at Gunnison County’s residential housing stock based on assessor data.

- The **Primary Improvements Dashboard** highlights overall housing condition, quality, and market characteristics for main dwellings only.  
- The **All Improvements Dashboard** expands the analysis to include every residential improvement — offering a full picture of the built environment across Economic Areas 1, 2, 6, and 8.  
- A navigation button links both dashboards, allowing side-by-side comparison of trends between primary and secondary structures.

**Skills:**  
Data visualization • Web development • Data cleaning • UX layout • Public data communication • GitHub Pages deployment

**Results:**  
- The majority of primary residential structures are in **Average** or **Good** condition, with smaller shares rated **Very Good** or **Excellent**.  
- When including **all improvements**, total **assessed improvement value** across Gunnison County exceeds **$9.4 billion**, illustrating the scale of residential development countywide.  
- Condition distribution patterns align with **economic areas** — higher-condition properties cluster in Areas 1 and 6 (Gunnison & Crested Butte), while more varied conditions appear in rural areas.

---
  
## Education  
**Western State Colorado University**  
**Bachelor of Arts – Biology**  
*Gunnison, CO — 2013*

---

## Certificates  
The best way to showcase skills is by building real-world projects, but certifications reflect dedication to structured learning. Here are my current credentials:

- **Google AI Essentials** *(2024)*  
- **Google Data Analytics Professional Certificate** *(2024)*  
- **Good Clinical Practice Certification** *(2024)*

---

## Contact  
**Email:** elissa.esterlein@gmail.com  




