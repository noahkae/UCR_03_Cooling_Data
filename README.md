# UCR-02 Cooling Data Analysis
This repository contains the code to process UCR-02 data alongside a study of relevant cooling system parameters. The structure of the repository alongside brief descriptions follows:
```
UCR_03_Cooling_Data
├── README.md <-- current file
├── data_files <-- folder containing all data from Kenesto, unprocessed
├── processed_data <-- folder with all processed, thinned testing data
├── .gitignore <-- to ignore large folders
├── Filtered_Efficiency_Map.csv <-- A 3-D lookup table of motor efficiency values
├── study-endurance.ipynb <-- notebook for data analysis and graphing, pseudo-endurance run only
├── study-aero-runs.ipynb <-- notebook for data analysis and graphing, aero coasting runs only
├── data_cleaning.ipynb <-- notebook for data filtering, converting raw data to usable formats
├── radiator_airflow_analysis.ipynb <-- analysis of real airflow data as measured by pitot tubes on the car
└── air-flow-estimation.ipynb <-- estimation of airflow from heat transfer equations
```

This repository will be kept fairly organized for the purpose of revisiting conclusions in the future, and will (hopefully) serve as the basis for cooling related changes on the UCR-03. All theory used is to be documented in the relevant notebooks.