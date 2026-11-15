# Engineering Notebooks

Python notebooks on process modeling, numerical methods and data analysis.

## About this repository

I am a process engineer (Warsaw University of Technology) working on hydraulic models of water and sewer networks. This repository is my workshop: I take a problem, write down the physics or mathematics behind it, solve it in Python and check whether the result makes sense.

The notebooks show how I work:

- turning a physical or biological process into equations and solving them numerically,
- collecting, cleaning and analysing real measurement data,
- understanding the methods I use, from statistics and machine learning to vector calculus.

Many topics are close to my professional field: wastewater treatment, rainfall and river data, flows.

These are learning and exploration notebooks, not production software. I wrote them myself, line by line, during self-study in 2021–2023 (textbooks and online courses, including Coursera), before AI coding assistants existed. In 2026 I collected them here and reviewed them for bugs and terminology.

## Projects

### Process modeling

- **[Methane fermentation (ADM1)](projects/adm1-methane-fermentation.ipynb)**: anaerobic digestion of wastewater sludge with ADM1, the IWA standard model for anaerobic digesters (27 differential equations, stiff solver LSODA in SciPy). Substrates, intermediates, biomass and biogas flow over time.
- **[Semibatch reactor](projects/semibatch-reactor-balance.ipynb)**: coupled mass and energy balance of a semibatch reactor with reactant dosing. Isothermal operation compared with no cooling under an exothermic reaction.

### Data collection and analysis

- **[IMGW weather archive](projects/imgw-data-downloader.ipynb)**: automated download of archived hydrological and meteorological data from IMGW-PIB (water levels, flows, precipitation, temperature, wind) for a chosen period and set of parameters. Public data of the kind used as input for urban drainage and river models.
- **[Weather prediction](projects/weather-prediction-regression.ipynb)**: predicting visibility from temperature, humidity, pressure, time of day and precipitation. Data cleaning, one-hot encoding of weather phenomena and scaling, then a neural network compared with a random forest.
- **[California traffic collisions](projects/traffic-collision-sql-geospatial.ipynb)**: SQL queries on the SWITRS SQLite database (aggregations, subqueries, date functions), a county-level choropleth map in Folium and Plotly charts.

## Foundations

Shorter notebooks on statistics, machine learning and mathematics, partly from coursework: the groundwork behind the projects above.

- **[Heart disease data](foundations/heart-disease-visualization.ipynb)**: exploratory analysis of categorical and numerical features. Associations between categorical features measured with Cramér's V, separately for patients with lower and higher heart attack risk.
- **[Overview of ML algorithms](foundations/ml-algorithms-overview.ipynb)**: seven algorithms on simple data, covering classification (k-NN, naive Bayes, decision tree), regression (linear, polynomial), clustering (k-means) and anomaly detection (One-Class SVM).
- **[Iris classification](foundations/iris-classification-cross-validation.ipynb)**: decision tree, k-NN, SVM and a neural network compared with repeated k-fold cross-validation.
- **[Coefficient of determination](foundations/coefficient-of-determination.ipynb)**: R² calculated from its definition in NumPy, including the case of three variables. Logarithmic and quadratic relationships are linearized and the results are checked against scikit-learn.
- **[Complex numbers](foundations/complex-numbers.ipynb)**: algebraic and trigonometric forms, arithmetic, powers and roots (de Moivre's formula), visualized on the complex plane.
- **[Differential operators](foundations/differential-operators.ipynb)**: gradient, divergence and curl calculated symbolically with SymPy and plotted as vector fields.

## Tools

Python · NumPy, pandas · SciPy, SymPy · scikit-learn · matplotlib, seaborn, Plotly, Folium · SQLite

## Data

Datasets are not included in the repository. Each notebook links to its data source.

## Contact

krystian.molenda@outlook.com
