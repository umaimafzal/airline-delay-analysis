# Airline Delay Analysis (2013–2023)

Author:Umaima Afzal  
Contact: [LinkedIn](https://www.linkedin.com/in/YOUR-LINK) | [Medium Article](https://medium.com/YOUR-MEDIUM-LINK)  

---

 Overview
This project analyzes 171,000+ records of U.S. airline delays (2013–2023) using FAA/BTS reporting schema.  
The goal was to uncover systemic inefficiencies in U.S. aviation by combining descriptive analytics, visualizations, and predictive modeling.  

---

 Data
- Source: Public dataset from [Kaggle](https://www.kaggle.com) harmonized with the U.S. Department of Transportation’s Bureau of Transportation Statistics (BTS) schema.  
- Records: 171,666 rows of monthly observations at the airport–carrier level.  
- Variables include:
  - Operational: airport code, carrier code, month, year, arriving flights.  
  - Delay indicators: delays >15 minutes, cancellations, diversions.  
  - Delay causes (minutes): carrier, weather, NAS, security, late aircraft.  
- Alignment: Consistent with the FAA’s causal taxonomy (FAA, 2024).  

---

 Methodology
- Cleaning: Minimal missingness (~0.2%). Validated carrier and airport codes against BTS documentation.  
- Feature Engineering: Delay rates, cause shares, lagged delay variables.  
- Tools: Python (pandas, NumPy, matplotlib, seaborn, squarify, scikit-learn).  
- Modeling: Logistic Regression & Random Forest classifiers for “high-delay months.”  
- Evaluation: ROC-AUC, precision/recall, F1-score, confusion matrices.  



 Key Findings
1. Late-aircraft propagation is the biggest driver (40–60% of total delay minutes).  
2. Carrier inefficiencies and NAS congestion outweigh weather as systemic causes.  
3. Regional carriers are disproportionately affected at congested hubs.  
4. Airports like Newark (EWR), O’Hare (ORD), and San Francisco (SFO) are recurring bottlenecks.  
5. Machine Learning models (Random Forest AUC = 0.83) show that past delays strongly predict future delays.  



 Why It Matters
- For airlines: Build resilience with schedule buffers, dynamic rotations, predictive resource allocation.  
- For airports & FAA: Target modernization at bottlenecks (EWR, ORD, SFO) to reduce NAS congestion.  
- For passengers: Delays are systemic, not random — plan itineraries accordingly.  

At scale, flight delays affect national productivity, infrastructure resilience, and U.S. economic competitiveness.  



 Repository Contents
- `flight_delay.ipynb` → Full Jupyter Notebook with cleaning, analysis, visualizations, and models.  
- `README.md` → Project overview (this file).  
- *(Optional)* `Airline_Delay_Cause.csv` → Dataset (https://www.kaggle.com/datasets/ryanjt/airline-delay-cause)

---

 References
- Bureau of Transportation Statistics (BTS). (2023). Airline On-Time Statistics.  
- Federal Aviation Administration (FAA). (2024). NextGen Annual Report.   
- Ball, M. et al. (2010). Total Delay Impact Study. U.S. DOT.  

---

 Links
- Full write-up on Medium: [Medium Article](https://medium.com/@afzalumaima26/what-10-years-of-u-s-airline-delays-reveal-about-systemic-inefficiencies-in-american-aviation-006804a4b2dd)  
- Connect with me: [LinkedIn](https://www.linkedin.com/in/umaimaafzal/)  

---

# License
This repository is provided for educational and research purposes.
