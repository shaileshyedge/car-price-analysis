
# What Drives the Price of a Used Car?

## Summary
This project analyzes a dataset of 426,000 used car listings to understand what factors make a car more or less expensive. The analysis follows the CRISP-DM framework and provides clear
recommendations to a used car dealership on how to fine-tune their inventory.

## Link to Notebook
[prompt_II.ipynb](prompt_II.ipynb)

## Key Findings
After building and comparing three regression models (LinearRegression, Ridge, and Lasso), the following key price drivers were identified:

**Factors that increase price:**
- Newer model year — the single strongest predictor of price
- Low odometer reading — fewer miles means higher value
- Good or excellent condition — reconditioning pays off
- Clean title — salvage/rebuilt titles significantly reduce value

**Factors that decrease price:**
- High mileage — more miles means lower price
- Older model year — depreciation is significant
- Salvage or rebuilt title — buyers pay much less for these

## Best Model
Ridge Regression performed best with:
- **RMSE: $5,817** — predictions within ~$5,817 on average
- **R²: 0.837** — explains 83.7% of price variation

## Recommendations for the Dealership
1. Focus on acquiring newer, low mileage vehicles
2. Avoid salvage and rebuilt title cars unless at steep discount
3. Invest in reconditioning cars to good/excellent condition
4. Use the Ridge Regression model as a pricing tool for new inventory

## Next Steps
- Collect more complete data for condition and cylinders
- Retrain the model periodically as market conditions change
- Consider adding make/model popularity as a feature

## Files
- `prompt_II.ipynb` — Full analysis notebook
- `data/vehicles.csv` — Dataset

## Tools Used
- Python, Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn (Linear Regression, Ridge, Lasso, GridSearchCV, Pipeline)

