# UCR-02 Cooling Data Analysis
This repository contains the code to process UCR-02 data alongside a study of relevant cooling system parameters. The structure of the repository alongside brief descriptions follows:
```
UCR_03_Cooling_Data <-- this repository
├── README.md <-- current file
├── data_files <-- folder containing all data from Kenesto
├── processed_data <-- folder with all processed, thinned testing data
├── data_cleaning.ipynb <-- notebook for data filtering
├── study.ipynb <-- notebook for data analysis and graphing
└── using_git.md <-- a brief guide on using git for unfamiliar members
```

This repository will be kept fairly organized for the purpose of revisiting conclusions in the future, and will (hopefully) serve as the basis for cooling related changes on the UCR-03. All theory used is to be documented in the relevant notebooks.

**If you are unsure of how to use git or why git is used, please refer to the using_git.md file.** This project should serve as a source of information for future members working on cooling systems.

TODO:
- [x] Analyze $\eta$ of endurance
- [x] Analyze $\eta$ of constant rpm aero runs
- [ ] Analyze $\eta$ of 2024 data <- Can't, doesnt have motor torque/rpm
- [ ] Compare $\eta$ over years and conclude in a single notebook <- 2024 Data is incomplete
- [x] Review radiator testing data
- [x] Estimate $h_{rad}$; quick estimate from excel, $hA_{rad}$ combined term is ~241, curve cant be assembled without $\dot{m}_{air}$ variance
- [ ] Analyze $\Delta T_{air} and \dot{m}_{air}$
- [ ] Compile results and adjust Simulink model accordingly