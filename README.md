# Shipment Prediction

Predict the next booking date and shipment type for each company using historical booking data (2021–2025).

# Approach

# 1. Baseline (Primary Solution)
- Next Booking Date: Weighted moving average of recent booking gaps  
- Shipment Type: Mode over recent 90-day window  

This approach prioritizes:
- Recency
- Stability
- Interpretability  

# 2. Machine Learning 
- Random Forest classifier using:
  - Time features (day, month)
  - Previous shipment type
  - Company encoding  

Used to evaluate if ML adds predictive value.

# Key Findings

- Shipment patterns are frequency-dominated
- Random Forest predictions closely match baseline
- Limited feature space → weak ML signal

# Conclusion

A recency-weighted statistical approach performs comparably to ML while being:

- Simpler  
- Faster  
- More interpretable  
