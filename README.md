# GeM Bid Data Extraction & Analysis

## Overview

This project provides a robust and scalable solution to **extract, deduplicate, and analyze bid data** from the **Government e-Marketplace (GeM)** portal.

The GeM portal uses **JavaScript-driven pagination with unstable ordering**, which makes traditional scraping approaches unreliable. This project addresses those challenges by using **real browser automation**, **DOM-based synchronization**, and **on-the-fly deduplication** to ensure accurate and complete data collection.

The extracted data is stored in a clean, reusable CSV format and can be used for further analysis, reporting, and dashboarding.

---

## Key Features

- Real browser automation for JavaScript-rendered pages  
- Handles unstable and reshuffled pagination reliably  
- Extracts only **unique bids** using Bid Number as the primary key  
- Incremental CSV persistence for long-running jobs  
- Safe restart and recovery without data loss  
- Designed for large-scale data extraction (tens of thousands of bids)  
- Output ready for downstream analysis and UI visualization  

---

## Data Extracted

For each unique GeM bid, the following fields are captured:

- **Bid Number**
- **Item Description** (full list via tooltip data)
- **Quantity**
- **Department Name and Address**
- **Bid Start Date**
- **Bid End Date**

The final dataset is stored as a CSV file:

 testing
