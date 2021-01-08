# EDA-Metis Project 1

**WomenTechWomenYes Street Team Analysis and Recommendations**

**Description of project goals**

Our first Metis project was focused on data cleaning and exporatory data analysis (EDA). We were tasked with optimizing street team placement at MTA subway entrances to maximize awareness and reach for WTWY fundraising efforts and summer gala.

**Features and Target Variables:**

- MTA Stations with high foot traffic volumes
    - Looked at both daily and weekly trends from 03/23/19-06/01/19
- Areas of high female population density
- Areas of high median incomes
- Areas where teh population has advanced degrees

- A weighted algorithm was used to determine target stations that met all these criteria
- Daily foot traffic trends for all stations were used to determine best days of week for street team implementation

**Data Used**
- MTA Data from 03/23/19-06/01/19
- American Community Survey Data focusing on Census tracts for our target demographics
- NYC Open Data for the MTA station locations/coordinates

**Tools Used**
- Numpy
- Pandas
- Pickle
- Matplotlib
- Seaborn
- Geopy/Geopandas
- FuzzyWuzzy

**Possible impacts of your project**
- Impacts in the scope of the project:
    - Determination of improved street team placement
    -Concepts of how to future optimize street team placement

- Personal/Professional impacts:
    - Developing an understanding of different python pacakges
    - Experience working on a data science project as part of a team
    - Experience presenting a data science project to an audience
    
**Guide to our Repo**
Project Slides
- Metis Project 1.pdf

MTA Data
- MTA initial cleaning, EDA, and visualization
    - Jupyter Notebook:
        - MTA_EDA.ipynb
    - Image files:
        - TURNSTILE_DAILY_ENTRIES.svg
        - GRD_CNTRL_DAILY.svg
        - GRD_CNTRL_DAILY_BY_WEEK.svg
        - TOP_STATIONS.svg
        - BUSIEST_DAY.svg

ACS Census Data
- Education
    - Data files:
        - Education_data_with_overlays.csv
        - Education_metadata.csv
    - Jupyter Notebook:
        - Education.ipynb
    - Pickle export:
        - Df_education.pkl
- Gender_age
    - Data files:
        - gender_age_data_with_overlays.csv
        - Gender_age_metadata.csc
    - Jupyter Notebook:
        - Gender_age.ipynb
    - Pickle export:
        - Df_gender_age.pkl
- Combine gender_age and education
    - Import files:
        - df_education.pkl
        - Df_gender_age.pkl
    - Jupiter notebook:
        - Census.ipynb
    - Pickle export:
        - Df_census.pkl


Merge MTA data with NYC Open Data/Census Data
- Import files:
    - Final_mta_v1.pkl
    - nyc_open_data_subway.csv
- Jupyter notebook:
    - mta_nyc_open_match.ipynb
- Export:
    - Final_merge_v2.csv