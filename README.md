# nasa-website-1995-analysis

This is a personal project aimed at gleaning insights to a sample 1995 NASA web access log publicly available in https://ita.ee.lbl.gov/html/contrib/NASA-HTTP.html

The two main goals or problem statement to answer here:
1. Can the data be used to identify behaviour patterns which can be used to optimise customer experience?
2. Can the data provide reason in difficulty finding content (e.g. identify 404 patterns) which can be used to improve navigation experience?

## How to start:

The raw logs used are (must be included in the /data/raw/ folder):
1. [Jul 01 to Jul 31, ASCII format, 20.7 MB gzip compressed](ftp://ita.ee.lbl.gov/traces/NASA_access_log_Jul95.gz)
2. [Aug 04 to Aug 31, ASCII format, 21.8 MB gzip compressed](ftp://ita.ee.lbl.gov/traces/NASA_access_log_Aug95.gz)

Starting folder structure for analysis (new files will be created as the notebook cells are run):
```
NASA-WEBSITE-1995-ANALYSIS
    |__ data
        |__ cleaned
        |__ processed
        |__ raw
            |__ NASA_access_log_Aug95 (extracted file from gz raw log)
            |__ NASA_access_log_Jul95 (extracted file from gz raw log)
    |__ eda
        |__ nasa_website_analysis.ipynb (notebook file)
```

## Progression:
Analysis approach taken at a high-level *(discussed in /eda/nasa_website_analysis.ipynb notebook)*:
1. [DONE] Understanding the variables
2. [DONE] Cleaning dataset and identifying features
3. [WIP] Identifying relationship between features
4. [NOT STARTED] How to optimise customer experience (using gleaned feature relationships)
