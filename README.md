# Parking-Tickets-CS4002-ThunderPandas
## This repository supports the Parking Ticket Prediction project by Team Thunder Pandas. The goal of the project is to use data to forecast parking violations in Charlottesville on a street-level view. This repository is organized for reproducibility and clarity, following best practices for open data science projects. It contains all scripts, data documentation, outputs, and supporting files needed to understand, reproduce, and extend the analyses.

# Software and Platform
This project was developed and tested using Python 3 in Google Colab (cloud Linux environment), but can be run locally on any modern Windows, Mac, or Linux machine with the necessary Python packages installed.

**Primary software and libraries:**

- Python 3.8+ (tested on Google Colab)
- scikit-learn
- pandas
- matplotlib
- seaborn
- transformers 

To set up all dependencies, refer to requirements.txt or manually install these packages using pip:

# Section 2: Documentation

├── README.md # Project orientation and reproduction instructions


├── LICENSE.md # MIT License for all code in this repository


├── SCRIPTS/

│ ├──   Script1_time_series_analysis.ipynb

│ ├──   Script2_hotspot_prediction_model.ipynb

│ ├──   requirements.txt


├── DATA/


│ ├──     Metadata.md

│ ├──     Number of Tickets.png

│ ├──     Parking_Tickets.csv

│ ├──     Tickets by Hour.png


├── OUTPUT/

│ ├──     feature_importance.csv

│ ├──     feature_importance.png

│ ├──     final_predictions.csv

│ ├──     model_comparison_rmse.png

│ ├──     model_performance_metrics.csv

│ ├──     poisson_predictions_vs_actual.png

│ ├──     residual_plot.png


# Section 3: Reproduction
To reproduce the results in this repository, follow these steps:
1. **Clone this repository:**

```
git clone https://github.com/nathanktran/Parking-Tickets-CS4002-ThunderPandas.git
cd Parking-Tickets-CS4002-ThunderPandas
```

2. **Set up the Python environment:**
In the scripts folder, access requirements.txt and run:
```
pip install -r requirements.txt
```
Otherwise, install dependencies manually (see Software and Platform)

3. **Acquire the data**
- If Parking_Tickets.csv is available in the DATA/ folder, no further action needed
- If the data is too large to store on GitHub, follow the instructions in DATA/Metadata.md to download the original Parking Ticket dataset from the [City of Charlottesville](https://opendata.charlottesville.org/search?q=parking%20tickets)

4. **Run all scripts in order**
- Change into the SCRIPTS/ directory, and run each numbered script sequentially to clean the data, engineer features, train models, and evaluate.
- Each script is heavily commented and includes header docstrings describing functionality and expected inputs/outputs.

5. **View results**
- All output files (accuracy scores, plots, and tables) will be automatically generated in the OUTPUT/ folder


