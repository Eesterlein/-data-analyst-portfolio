# Elissa Esterlein – Data Analyst Portfolio

Interactive portfolio highlighting data projects, dashboards, and public-facing tools across analytics, automation, and web development.

---

## About

Hi, I’m Elissa Esterlein — a data analyst with a background in biology and medical research and a strong interest in applying data-driven insights to public policy, housing, land use, and community systems.

My work spans exploratory analysis, dashboards, internal automation tools, and lightweight web applications. I’m especially interested in transparency, reproducibility, and designing tools that make complex systems easier to understand for both technical and non-technical users.

I’m actively building through real-world projects, certifications, and public datasets, and I’m excited to contribute to mission-driven organizations as a thoughtful, adaptable data analyst.

📍 Based in Colorado  
📁 View my resume: [CV_pdf.pdf](CV_pdf.pdf)  
📊 [Kaggle](https://www.kaggle.com/elissaesterlein) • [Tableau Public](https://public.tableau.com/app/profile/elissa.esterlein/vizzes) • [GitHub](https://github.com/Eesterlein)

---

## Portfolio Projects

### Table of Contents

- [About](#about)

- [Workplace Automation & Internal Tools](#workplace-automation--internal-tools)  
  - [Local LLM Knowledge Assistant](#local-llm-knowledge-assistant)  
  - [MLS Photo Processor](#mls-photo-processor)  
  - [Gunnison County Property Analysis Map](#gunnison-county-property-analysis-map)  
  - [Zillow Property & Photo Scraper](#zillow-property--photo-scraper-in-development)
  - [Gunnison County Map Explorer](#gunnison-county-map-explorer)

- [Data Analysis & Research](#data-analysis--research)  
  - [Garmin Fitness Data Analysis](#garmin-fitness-data-analysis)  
  - [Colorado Land Ownership](#colorado-land-ownership)  
  - [US State-level Demographics Snapshot](#us-state-level-demographics-snapshot)

- [Dashboards & Data Storytelling](#dashboards--data-storytelling)  
  - [Gunnison County Housing Dashboard (Pre/Post COVID)](#gunnison-county-housing-dashboard-prepost-covid)  
  - [Residential Structure Conditions in Gunnison County](#residential-structure-conditions-in-gunnison-county)

- [Web Applications & Public Tools](#web-applications--public-tools)  
  - [Gunnison Airport Flight Tracker Website](#gunnison-airport-flight-tracker-website)  
  - [Gunnison County Property Tax Calculator](#gunnison-county-property-tax-calculator)

- [Education](#education)  
- [Certificates](#certificates)  
- [Contact](#contact)


---

## Workplace Automation & Internal Tools

### Local LLM Knowledge Assistant
**Code:** https://github.com/Eesterlein/Building-Local-LLMs-for-Private-Workflows

**Goal:**  
Demonstrate how organizations can deploy private, on-device AI assistants for internal knowledge use without exposing data to third-party APIs.

**Description:**  
Built a locally hosted LLM chatbot using Ollama and LlamaIndex that simulates an internal policy assistant trained on company handbooks and PDFs. The tool uses retrieval-augmented generation (RAG) to answer questions entirely offline, making it suitable for sensitive or regulated environments.

**Skills:**  
Prompt engineering • Vector indexing • RAG pipelines • Local AI deployment • Knowledge systems design

**Technology:**  
Python, Ollama, LlamaIndex, LangChain, Markdown  
*(FastAPI integration planned)*

**Results:**  
Delivered a working proof-of-concept showing how organizations can replace cloud-based chat tools with private, auditable AI assistants while maintaining strong answer quality.

---

### MLS Photo Processor
**Code:** https://github.com/Eesterlein/MLS-Photo-Processor  

**Goal:**  
Automate the renaming, sorting, and classification of MLS property photos for assessor and appraisal workflows.

**Description:**  
A local desktop utility that matches user-provided parcel numbers to internal account records and uses a vision-language model (CLIP) to automatically classify photos (e.g., Kitchen, Exterior, Bathroom). The tool converts unstructured, randomly named downloads into standardized, system-ready files with no manual data entry.

**Skills:**  
Zero-shot image classification • Desktop GUI development • File system automation • Data mapping

**Technology:**  
Python, PyTorch, Hugging Face (CLIP), Pandas, Tkinter, Pillow

**Results:**  
Eliminated manual renaming for high-volume photo sets. The tool uses conservative classification, defaulting to “Other” when confidence is low, ensuring reliable file naming compatible with local government systems.

---

### Gunnison County Property Analysis Map
**Code:** https://github.com/Eesterlein/gunnison_gis_mapping_static_demo  
**Live Demo:** https://eesterlein.github.io/gunnison_gis_mapping_static_demo/html_map/

**Goal:**  
Provide appraisers and GIS analysts with a fast, visual method to identify data gaps and valuation inconsistencies across Gunnison County.

**Description:**  
A lightweight web mapping application that joins assessment CSVs with GeoJSON parcel boundaries. Users can dynamically style parcels by quality, view, or value to surface missing or outlier data during valuation review.

**Skills:**  
Geospatial joins • Thematic mapping • Front-end web development • Data QA

**Technology:**  
JavaScript (ES6+), Leaflet.js, HTML5/CSS3, GeoJSON, CSV

**Results:**  
Achieved 97% parcel coverage by merging multiple data sources, enabling faster spatial auditing of county property records.

---

### Zillow Property & Photo Scraper *(In Development)*
**Code:** https://github.com/Eesterlein/zillow-photo-scraper-scraperapi  

**Goal:**  
Automate extraction of property metadata and images from Zillow for appraisal and market analysis.

**Description:**  
A Python-based scraping utility using ScraperAPI to retrieve listing data and images, with fuzzy address matching to auto-organize downloads into account-level folders. Currently being refactored to use Playwright + Chromium for improved stability.

**Skills:**  
Web scraping architecture • API integration • Data normalization • Asset automation

**Technology:**  
Python, Requests, Pandas, JSON, BeautifulSoup (Playwright planned)

**Results:**  
Built a batch-processing pipeline that significantly reduced manual effort for compiling subject property photo sets.

---

### Gunnison County Map Explorer
**Code:** https://github.com/Eesterlein/gunnison-county-map-explorer

**Goal:**  
Build a modern, interactive GIS map to support internal property assessment workflows by providing fast, intuitive access to parcel, jurisdiction, and town-level spatial data.

**Description:**  
Designed and implemented a full-stack GIS web application that serves county assessor shapefiles through a PostGIS database and exposes them via an OGC API – Features service. Spatial data is containerized and served using Docker, with TBG (Tiny Building Blocks) providing standards-compliant vector tile delivery.

The frontend is a React + TypeScript application built with MapLibre GL, allowing users to toggle assessment layers, switch base maps (street, satellite, terrain), and smoothly navigate to predefined towns using animated map transitions. The architecture cleanly separates base maps from vector layers, ensuring performance and maintainability as datasets grow.

This project demonstrates how legacy GIS data can be transformed into a modern, web-native mapping tool suitable for internal government use, without reliance on proprietary GIS platforms.

**Skills:**  
GIS systems design • Spatial databases • OGC standards • Web mapping • Frontend architecture • Dockerized services

**Technology:**  
PostgreSQL / PostGIS • OGC API – Features (tipg) • TBG (vector tile server) • Docker & Docker Compose • React • TypeScript • MapLibre GL • Vite

**Results:**  
Delivered a performant, extensible GIS application that enables interactive exploration of property and jurisdiction data, providing a foundation for future assessor tools such as valuation overlays, parcel analytics, and public-facing map views.

---

## Data Analysis & Research

### Garmin Fitness Data Analysis
**Code:** https://github.com/Eesterlein/My-2024-Garmin-Data-Analysis-  
**Live Report:** https://eesterlein.github.io/My-2024-Garmin-Data-Analysis-/

**Goal:**  
Identify patterns and seasonality in personal health and fitness data.

**Description:**  
Analysis of activity, calories, heart rate, sleep, and stress data across 2024, focusing on correlations, seasonal trends, and wellness indicators.

**Skills:**  
Data wrangling • Time series analysis • Statistical correlation • Data storytelling

**Technology:**  
Python, Pandas, Matplotlib, Seaborn

**Results:**  
Found a strong correlation between activity and calorie burn (0.89), seasonal changes in workout intensity, and a moderate relationship between stress and resting heart rate.

---

### Colorado Land Ownership
**Code:** https://github.com/Eesterlein/colorado-land-ownership  
**Live Report:** https://eesterlein.github.io/colorado-land-ownership/

**Goal:**  
Analyze public vs. private land ownership across Colorado and identify absentee ownership patterns.

**Description:**  
Combined COMaP shapefiles, parcel data, and assessor records to visualize ownership by agency, residency, and entity type.

**Skills:**  
Geospatial analysis • Public land data • Mapping • Data cleaning • Storytelling

**Technology:**  
Python, GeoPandas, Matplotlib, ArcGIS, GitHub Pages

**Results:**  
Identified that 62.6% of Colorado land is privately owned; in Gunnison County, over 76% is public, while private parcels show increasing out-of-county ownership.

---

### US State-level Demographics Snapshot
**Code:** https://github.com/Eesterlein/us-state-demographics-sql-acs2019  
**Dashboard:** https://lookerstudio.google.com/s/mNjbN_gsXoQ

**Goal:**  
Analyze state-level socioeconomic indicators using U.S. Census ACS data.

**Description:**  
Used SQL to calculate and rank poverty, income, unemployment, education, and rent burden metrics. Visualized results in Looker Studio with interactive maps and scorecards.

**Skills:**  
SQL • CTEs • Window functions • CASE logic • Dashboard design

**Technology:**  
BigQuery, Looker Studio, Google Cloud Console

**Results:**  
Produced a national dashboard highlighting disparities in income, education, and housing affordability across all U.S. states.

---

## Dashboards & Data Storytelling

### Gunnison County Housing Dashboard (Pre/Post COVID)
**Code:** https://github.com/Eesterlein/gunnison-housing-snapshots  
**Live Site:** https://eesterlein.github.io/gunnison-housing-snapshots/

**Goal:**  
Compare pre-COVID (2017–2018) and post-COVID (2022–2023) housing conditions in Gunnison County.

**Description:**  
Single-page dashboard showing medians, price per square foot, sales volume, affordability estimates, and Gunnison vs. U.S. context.

**Results:**  
Median prices rose from $305k to $575k; affordability dropped from 42% to 14% of U.S. households.

---

### Residential Structure Conditions in Gunnison County
**Code:** https://github.com/Eesterlein/gunnison-residential-condition  
**Live Site:** https://eesterlein.github.io/gunnison-residential-condition/

**Goal:**  
Visualize assessed condition and value of residential structures across Gunnison County.

**Description:**  
Two linked dashboards comparing primary improvements vs. all residential improvements across economic areas.

**Results:**  
Showed condition clustering by economic area and over $9.4B in assessed residential improvement value countywide.

---

## Web Applications & Public Tools

### Gunnison Airport Flight Tracker Website
**Code:** https://github.com/Eesterlein/gunnison-airport-tracker  
**Live App:** Not currently hosted to limit API usage and ongoing hosting costs

**Goal:**  
Track real-time private and commercial flights near Gunnison Airport (KGUC).

**Description:**  
Web app integrating OpenSky Network API with PostgreSQL to log and display flight activity over time.

**Technology:**  
Node.js, Express, PostgreSQL, OpenSky API, Heroku

**Results:**  
Deployed a working flight tracker that logs repeat aircraft sightings and updates hourly.

---

### Gunnison County Property Tax Calculator
**Code:** https://github.com/Eesterlein/gunnison-county-property-tax-calculator  
**Live Tool:** https://eesterlein.github.io/gunnison-county-property-tax-calculator/

**Goal:**  
Provide a clear, educational estimate of property taxes in Gunnison County using publicly available assessment data.

**Description:**  
A fully client-side web application that calculates estimated property taxes based on actual value, assessment rates, and mill levies. The tool mirrors real-world government workflows while remaining transparent and easy to understand for property owners.

Includes logic for residential, commercial, vacant land, and applicable exemptions, with clear disclaimers around rounding differences and official tax systems.

**Skills:**  
Business logic translation • Data validation • UX clarity • Public-facing tool design

**Technology:**  
HTML, CSS, JavaScript, JSON, GitHub Pages

**Results:**  
Delivered a production-ready educational tool that improves transparency and reduces confusion around how property taxes are calculated.

---

## Education

**Western Colorado University**  
Bachelor of Arts – Biology  
Gunnison, CO (2013)

---

## Certificates

- Google AI Essentials (2024)  
- Google Data Analytics Professional Certificate (2024)  
- Good Clinical Practice Certification (2024)

---

## Contact

📧 elissa.esterlein@gmail.com




