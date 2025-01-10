# ThermoG v0.1: User Tutorial

## 1. Data Preparation

Before running the ThermoG algorithm, it's crucial to prepare your input data correctly. Here's what you need to know:

**Key Requirement:**
- Gravity anomaly data, such as Bouguer anomaly, must be provided in a coordinate system with metric units to ensure consistent spatial calculations and maintain accurate grid resolution.

**Recommended Coordinate System:**
- **Mercator WGS84** - EPSG code: **3395** (WGS 84 / World Mercator projection)
  - This projection ensures that coordinates are in meters, which is vital for accurate calculation of grid and temperature distribution.

**Input File Format:**
- The algorithm expects input data in **CSV** format with the following structure:
  
  X, Y, Bouguer

  100000, 200000, -150.3
  
  100500, 200500, -145.2
  

  - **X**: Easting coordinate in meters.
  - **Y**: Northing coordinate in meters.
  - **Bouguer**: Bouguer anomaly values in mGal.

## 2. Software Environment

ThermoG can be executed in Python environments with the following specifications:

**Python Installation:**
- **Python 3.8 or higher** should be installed on your system.
- Required libraries:
  - `numpy`
  - `pandas`
  - `matplotlib`
  - `scipy`

  Install these libraries using pip:

  ```bash
  pip install numpy pandas matplotlib scipy

Jupyter Notebook:
For an interactive experience, ThermoG can be run within a Jupyter Notebook.

Google Colab:
ThermoG is primarily designed for Google Colab. 
Upload this notebook directly to your Google Drive, then open it in Google Colab to run. Here's how:
Upload to Google Drive: Save the ThermoG notebook file to your Google Drive.
Open in Colab: Navigate to Google Colab, click on "File" > "Open notebook", then "Google Drive" to select and open your ThermoG notebook.
Execute: Run each cell of the notebook sequentially. Ensure your input data (CSV file) is accessible from your Google Drive or uploaded directly to Colab.

Note: Make sure all your data files are correctly formatted and in the right place before running the ThermoG script. If you encounter any issues, please check your data format first.
