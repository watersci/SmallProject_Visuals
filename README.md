### **README: USGS Water Quality Dashboard in R**

## **Overview**
This Shiny app provides an interactive way to **retrieve and visualize** instantaneous USGS water quality data from the **USGS National Water Information System (NWIS)**. 

Users input a **USGS Site ID**, retrieve **available water quality parameters**, and generate a **time-series plot and data table** based on the chosen parameter.

🔗 **Find your USGS Site ID here:** [USGS Water Data Mapper](https://maps.waterdata.usgs.gov/mapper/index.html)

---

## **How It Works**
1. **Enter a USGS Site ID** (e.g., `"01463500"`) in the input field.
2. Click **"Get Available Parameters"** to see which measurements are available.
3. **Select a parameter** from the dropdown menu.
4. **Set the date range**
5. Click **"Download Data"** to generate:
   - A **time-series plot** with a dynamically generated title.
   - A **data table** displaying the retrieved measurements.

---

## **Installation & Running the App**
### **Prerequisites**
Ensure you have the following R packages installed:
```r
install.packages(c("shiny", "dataRetrieval", "tidyverse", "DT", "lubridate", "ggplot2"))
```

---

## **Key Features**
✅ **Interactive UI**: Easily select sites and parameters.  
✅ **Real-Time Data Retrieval**: Uses the `dataRetrieval` package to fetch USGS data.  
✅ **Dynamic Plot Titles**: Displays the **official parameter name** for better readability.  
✅ **Simple & Customizable**: Modify the script to include additional parameters.  

---

## **Customization**
### **Adding More Parameters**
To expand the list of retrievable parameters, edit the `selectInput()` function in the **UI section** and modify `get_available_params()` accordingly.

---

## **Contributing**
Have suggestions or improvements? Feel free, this was done just for fun and to learn more about **Shiny**

---

## **Acknowledgments**
This project leverages the **USGS NWIS API** via the `dataRetrieval` package. Thanks to the **USGS** for providing open-access hydrological data!

---

