# Mobile Phone Price Prediction Project

This project focuses on predicting the **price range category** of mobile phones based on various hardware and connectivity features. Using a dataset containing specifications such as **battery power**, **RAM**, **camera megapixels**, **screen size**, **connectivity options** and many more, we train multiple machine learning models to classify phones into four price categories: 

- **0 = low cost**  
- **1 = medium cost**  
- **2 = high cost**  
- **3 = very high cost**

---

## Key Highlights

- **Dataset Features:**  
  The dataset includes the following mobile phone specifications:  

   **battery_power**: Battery Capacity in mAh  
   **blue**: Has Bluetooth or not  
   **clock_speed**: Processor speed (GHz)  
   **dual_sim**: Has dual SIM support or not  
   **fc**: Front camera megapixels  
   **four_g**: Has 4G or not  
   **int_memory**: Internal Memory in GB  
   **m_dep**: Mobile depth in cm  
   **mobile_wt**: Weight in grams  
   **n_cores**: Processor Core Count  
   **pc**: Primary Camera megapixels  
   **px_height**: Pixel Resolution height  
   **px_width**: Pixel Resolution width  
   **ram**: RAM in MB  
   **sc_h**: Mobile Screen height in cm  
   **sc_w**: Mobile Screen width in cm  
   **talk_time**: Time a single battery charge will last, in hours  
   **three_g**: Has 3G or not  
   **touch_screen**: Has touch screen or not  
   **wifi**: Has WiFi or not  


- **Feature Engineering:**  
  Created additional features such as:  
  - *resolution* 
  - *total camera megapixels*   
  - *battery-to-RAM ratio*  
  - *memory-to-RAM ratio*  
  - *core speed*   
  - *connectivity count*  
  - *talk time per battery power*

- **Models Evaluated:**  
  Logistic Regression, Random Forest, XGBoost, Support Vector Machine (SVM), K-Nearest Neighbors (KNN), and Gaussian Naive Bayes.

- **Final Model:**  
  Selected **Logistic Regression** for final deployment due to its high accuracy and interpretability, achieving over *97% accuracy* on the test dataset.

- **Prediction Output:**  
  The model outputs a **price category label** (e.g., *low cost*, *medium cost*, *high cost*, *very high cost*) for easy understanding.

---

## Usage

- Provide mobile specifications as input features in the required format.
- The trained model predicts the **price range category**.
- The output prediction is displayed with a descriptive label for better user interpretation.

### Python Version

- Python 3.12.5