# Project_Farglory-Home-Price-Prediction
### The client's requirement:
-Based on the market dataset and practice to build the home price prediction model with machine learning techs.
### Information summary:
- RFM : This is not suitable for the real estate industry with high unit price and high total price
- AARRR :The funnel of real estate is "documentation→new arrivals→revisiting→transaction"
- KANO's model : is also relatively unapplicable to real estate. The real estate market is not a consumer product or service industry.
### business flow:
"file → newcomer → revisit → transaction", there is already a BI report generated based on the CRM system inside.
Marketing Department can make suggestions on product planning and design. When the construction is planned, the real estate side will submit a market survey report near the base. When the construction plan is completed, the real estate will submit a "marketing report" for positioning to identify the potential buyers.
### The KPI:
The Marketing Director wants to use the historical dataset to find out what key variables affect sales, how it affects, how to measure it dynamically (upgrade the static BI function), and track the product price regularly to build price prediction model in one month.
### Our solution:
- To devise the machine learning system first, build machine learning models to rank clients feeds, we use the binary classification model coupled with custom loss function.
- Considering the datasize derived from CTR, we create the feed service which archive the feature store and item store, most of the feture stores built on mySQL clusters.
- Create the process to generate training data for formulating Machine Learning model.(As attached codes)
- We embedded the price estimator on the company webpage to provide better visualization on the Flask server.
- Scale out the feed service module designed.
**After the iterations of testing and scaling, the new data generated will loop back to optimize these models we built.**
