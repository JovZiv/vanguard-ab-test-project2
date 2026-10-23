# Vanguard A/B Test — Website Experience Analysis

## Project overview

This project evaluates whether Vanguard's redesigned website improves the client experience compared with the original website.

Clients in the **Control** group used the old website, while clients in the **Test** group used the new website. We compare the two groups using three key performance indicators (KPIs):

1. **Completion rate** — the proportion of clients who completed the process.
2. **Time efficiency** — elapsed time between recorded process actions, analysed by process step and age group.
3. **Error rate** — the frequency of errors during the process.

The analysis includes data cleaning and preparation, descriptive comparisons, statistical hypothesis tests, Tableau visualisations, and a final presentation. The results should be interpreted as comparisons between the experiment groups; observed differences do not by themselves prove why clients behaved differently.

## Project links

- **Trello project board:** https://trello.com/b/hBXWLNKa/project2-vanguard
- **Google Slides presentation:** [Open the presentation](https://drive.google.com/file/d/1uGgK8cC9nKdwf_PkPuLLfC2rTskZPxp0/view?usp=sharing)

### Tableau Public dashboards

Replace each placeholder with the published Tableau Public URL for the corresponding KPI dashboard:

- **Completion Rate:** [Completion Rate KPI](https://public.tableau.com/app/profile/jovana.zivkovic2133/viz/Completation-Rate-Vanguard-AB-Test/VanguardABtestdidthenewdesignhelpclientsfinish?publish=yes)
- **Time Efficiency:** [Time per Each Step KPI](https://public.tableau.com/app/profile/jovana.zivkovic2133/viz/vanguard-time/Dashboard1?publish=yes)
- **Error Rate:** [Error Rate KPI](https://public.tableau.com/app/profile/jovana.zivkovic2133/viz/Error-Rate-Vanguard-AB-Test/Dashboard1?publish=yes)

## Repository structure

The following structure reflects the project files shown in Visual Studio Code. Some files are intermediate or export datasets used during analysis and dashboard creation.

```text
vanguard-ab-test-project2/
├── tableau/
│   ├── age_group_tests.csv
│   ├── balance_check.csv
│   ├── ci_thresholds.csv
│   ├── clients_tableau.csv
│   └── hypothesis_tests.csv
├── df_clean.csv
├── df_clients.csv
├── df_final_demo.txt
├── df_final_experiment_clients.txt
├── df_final_web_data_pt_1.txt
├── df_final_web_data_pt_2.txt
├── df_tableau_time_client_level.csv
├── df_tableau_time.csv
├── README.md
├── vanguard_tableau_data.csv
└── vanguard-ab-test.ipynb
```

### Main files and folders

| File or folder | Purpose |
|---|---|
| `vanguard-ab-test.ipynb` | Main Jupyter notebook containing the analysis and results. |
| `df_final_demo.txt` | Source client demographic/profile data. |
| `df_final_experiment_clients.txt` | Source data identifying clients' experiment assignment. |
| `df_final_web_data_pt_1.txt`, `df_final_web_data_pt_2.txt` | Source website activity data supplied in two parts. |
| `df_clean.csv` | Cleaned website activity data used for analysis. |
| `df_clients.csv` | Client-level dataset used for completion-rate analysis, including fields such as experiment variation and completion status. |
| `df_tableau_time.csv` | Time-efficiency data prepared for Tableau. |
| `df_tableau_time_client_level.csv` | Time-efficiency data aggregated at client and process-step level for more consistent client-level comparisons. |
| `vanguard_tableau_data.csv` | Additional Tableau-ready dataset used in the project. |
| `tableau/` | Exported CSVs used to build or support the completion-rate Tableau analysis. |
| `tableau/age_group_tests.csv` | Test results comparing completion-related outcomes by age group. |
| `tableau/balance_check.csv` | Checks of balance between the experiment groups. |
| `tableau/ci_thresholds.csv` | Summary statistics and threshold values used for confidence-interval and practical-significance reporting. |
| `tableau/clients_tableau.csv` | Client-level data exported for Tableau. |
| `tableau/hypothesis_tests.csv` | Exported hypothesis-test results. |

## Getting the project in Visual Studio Code and Jupyter Notebook

### First time: clone the repository

Install Git and Python/Anaconda if they are not already available. Then open a terminal in Visual Studio Code and run:

```bash
git clone <GITHUB_REPOSITORY_URL>
cd vanguard-ab-test-project2
```

Replace `<GITHUB_REPOSITORY_URL>` with the actual repository URL. In VS Code, open the project folder and open `vanguard-ab-test.ipynb`. Select the Python environment/kernel that has the required packages installed.

## Presenters

1. **Presenter 1:** Effie
2. **Presenter 2:** Lena
3. **Presenter 3:** Jovana
4. **Presenter 4:** Fatma

