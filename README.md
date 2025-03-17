# 🦟 Fly Age Estimation via Image Processing  

## 📌 Overview  
This project aims to estimate the biological age of flies by analyzing the strength of their digestive system. Flies are fed a substance dyed blue, and its spread throughout their body serves as an indicator of digestive system integrity. A healthy fly retains the dye inside its digestive tract, while a weaker fly shows greater spread.  

To quantify this, we measure the **blue-to-red color ratio** in images of individual flies and use this as a proxy for dye distribution.  

---

## 🖥️ Project Structure  
This repository contains a **Google Colab Notebook** that automates the analysis in two main steps:  

### **1️⃣ Step 1: Threshold Visualization**  
Before running a full analysis, this step helps the user **choose the appropriate threshold** for blue/red ratio detection.  
- Randomly selects images from the dataset  
- Computes the **blue-to-red ratio**  
- Allows the user to **visually inspect the effects** of different threshold values  

### **2️⃣ Step 2: Full Image Analysis**  
Once a suitable threshold is chosen, the notebook processes **all images in a given folder**, extracting and summarizing the data.  
- Computes the **blue-to-red ratio** for each image  
- Identifies pixels where the ratio exceeds the selected threshold  
- Outputs:  
  - **Processed images** with ratio maps  
  - **Filtered images** highlighting relevant pixels  
  - **CSV file** summarizing results (pixel count, percentage, and image data)  

---

## 📂 Files in the Repository  
- `fly_analysis.ipynb` - The main **Google Colab Notebook** for running the analysis  
- `README.md` - This documentation  

---

## 🚀 How to Use  
### **1️⃣ Setup & Requirements**  
- The analysis is designed to run on **Google Colab**  
- Store your images in a **Google Drive folder**  

### **2️⃣ Running the Notebook**  
1. Open the [Google Colab Notebook](https://colab.research.google.com/)  
2. Upload your images to Google Drive  
3. Set the **image folder path** and **threshold value** in the notebook  
4. Run the cells and review the results  

---

## 📊 Expected Outputs  
- **Processed images** (`ratio_maps/`)  
- **Filtered images** (`filtered_pixels/`)  
- **CSV summary file** (`analysis_results.csv`)  

Each image is analyzed for its **blue-to-red ratio**, allowing comparisons across flies to assess their digestive health.  

---
