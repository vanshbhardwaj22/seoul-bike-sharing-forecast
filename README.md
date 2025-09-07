# Seoul Bike Sharing Demand Forecast

This project aims to forecast hourly bike rental demand in Seoul, South Korea, by building a predictive model that leverages key environmental and time-based factors. By moving beyond a simple analysis, this project culminates in a live forecasting tool that showcases an end-to-end machine learning solution.

# Methodology

The process began with a comprehensive approach to data understanding and preparation. The raw dataset, sourced from Kaggle, underwent thorough data cleaning and exploratory analysis to uncover key relationships between bike usage and variables such as temperature, humidity, and time of day. This was followed by a strategic feature engineering phase, where new features like "weekday" and "season" were created to provide the model with more predictive power.

With the data prepared, a methodical model selection process was undertaken. Several regression algorithms, including Linear Regression, Random Forest, and XGBoost, were evaluated to determine the best fit for the problem. The final model, an optimized XGBoost Regressor, was selected for its superior performance, as evidenced by its high R-squared score and low mean absolute error.

# Live Forecasting Implementation

The core differentiator of this project is its transition from static analysis to dynamic forecasting. A dedicated inference pipeline was built to load the pre-trained XGBoost model and its associated scaler. For real-time predictions, this pipeline was enhanced to seamlessly integrate with a live weather API. This allows the model to automatically fetch current weather conditions in Seoul, enabling a live, data-driven forecast of bike demand. This phase also involved solving crucial real-world challenges, such as handling API request formats, data types, and ensuring time zone accuracy.

# Results and Conclusion

The final model successfully achieved an R-squared score of 0.911 and a Mean Absolute Error (MAE) of 117.172 on the validation set, demonstrating its strong predictive capability. This accuracy is particularly valuable for a bike-sharing company, as it can be used to optimize bike distribution and ensure availability during peak demand hours. The project not only serves as a strong foundation for a full-scale deployment but also highlights the practical application of machine learning in a business context.
