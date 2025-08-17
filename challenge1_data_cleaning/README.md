# Challenge 1: Data Cleaning – Barcelona Airbnb Listings

## 🎯 Objective
Prepare the raw Barcelona Airbnb dataset for analysis by applying essential **data cleaning & feature engineering** techniques.

---

## 🛠️ Steps Taken
1. **Removed Unnecessary Features**  
   Dropped redundant columns (e.g., IDs, URLs, descriptions).  

2. **Standardized Data Types**  
   - Converted date columns (`host_since`, `first_review`, `last_review`) into proper `Date`.  
   - Converted boolean columns (`t/f`) into TRUE/FALSE.  
   - Converted price & cleaning_fee into numeric.  
   - Converted host_response_rate into numeric %.  

3. **String Cleaning**  
   - Lowercased all text.  
   - Removed accents using `stringi`.  

4. **Feature Engineering**  
   - Created boolean features for **host_verifications** (e.g., email, phone, government_id).  
   - Created boolean features for **amenities** (e.g., wifi, kitchen, elevator).  

5. **Simple Insights**  
   - Frequency table: `neighbourhood_group_cleansed × property_type`.  
   - Top amenities by frequency.  

---

## 📊 Key Results
- Dataset reduced to **19,833 listings** with **252 structured features**.  
- Most common property type: **apartments in Eixample & Ciutat Vella**.  
- Most frequent amenities: **WiFi, Essentials, Kitchen, Hangers, Washer/Dryer**.  

---

## 📂 Files
- `data_cleaning.R` – Full cleaning script  
- `amenities_freq.png` – Bar chart of most common amenities  
- `freq_table.png` – Property type frequency table  
