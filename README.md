 **ETL Pipeline: Extract, Transform, and Load Data**  

## **Overview**  
This project automates the **ETL (Extract, Transform, Load)** process by reading data from different file formats, processing it, and saving it in a structured format. The script is designed to handle CSV, JSON, and XML files, converting height and weight measurements into standardized metric units. Additionally, it maintains a log file to track the execution process.  


## **Features**  
- Automatically extracts data from multiple file formats (**CSV, JSON, XML**)  
- Converts **height (inches → meters)** and **weight (pounds → kilograms)**  
- Merges all extracted data into a single dataset  
- Saves the transformed data into a structured CSV file  
- Maintains a log file to track the progress and execution of the ETL process  

## **How It Works**  

### **1. Extraction Phase**  
The script scans the working directory for `.csv`, `.json`, and `.xml` files and extracts relevant data.  
- CSV files are processed as tabular data.  
- JSON files are read and structured appropriately.  
- XML files are parsed to extract necessary fields.  

### **2. Transformation Phase**  
After extracting the data, the script performs unit conversions:  
- **Height** is converted from inches to meters.  
- **Weight** is converted from pounds to kilograms.  
- The values are rounded to two decimal places for consistency.  

### **3. Loading Phase**  
Once the data is cleaned and transformed, it is saved into a single CSV file, making it ready for further analysis or integration into other systems.  

### **4. Logging Mechanism**  
A log file keeps track of every step in the process, ensuring transparency and aiding in debugging if any issues arise. Each step (extraction, transformation, loading) is recorded with timestamps.  


## **How to Use**  

1. Place all your CSV, JSON, and XML files in the same directory as the script.  
2. Run the script, and it will process the files automatically.  
3. The transformed data will be saved in a structured format for easy analysis.  
4. Check the log file for a detailed execution history.  

## **Customization**  
- The output file name can be changed based on user preference.  
- The script can be modified to include additional data transformations or new file formats.  
- The logging system can be enhanced for more detailed tracking.  

## **Conclusion**  
This ETL pipeline simplifies the process of handling multiple data formats, standardizing measurements, and consolidating information into a structured dataset. The automated logging ensures transparency and helps with monitoring the process. This project is useful for data processing, analytics, and integration into larger data workflows.  
