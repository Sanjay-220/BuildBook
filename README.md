# Marketing Mix Modelling (MMM) with Bayesian Regression

## Business Problem & Objective

An ecommerce brand selling athletic swimwear markets its products through platforms like Facebook, Google, TikTok, Email, and others. They also offer discounts to boost sales. Marketing managers aim to address the following questions:

- How much does each platform contribute to sales?
- What is the impact of discounts on sales?
- How do holidays drive sales?
- What is the effect of seasonality on sales?

## Approach

### Marketing Mix Modelling (MMM)

MMM is an econometric model designed to quantify the incremental impact of marketing and non-marketing activities on a target variable, such as sales.

![Picture2](https://github.com/user-attachments/assets/71aed094-98bd-4426-804d-02032069dc38)

#### Why not Linear Regression?
- **Non-linear sales relationships**: Accounts for lag effects and diminishing returns.
- **Time series components**: Considers trend and seasonality.
- **Collinearity**: Handles interdependencies among marketing variables.

#### Why Bayesian Regression?
- Leverages industry experience as Bayesian priors.
- Provides insights into both parameter and model uncertainty.

## Model Build

The model incorporates three transformation types:
1. **Adstock**
2. **Carryover**
3. **Hill-Adstock**

The transformation with the lowest Train and Test errors is chosen as the optimal one.

### Best Chosen Model:
- **Transformation**: Hill-Adstock
- **Performance**: ~90% R² and MAPE of 10%

## Model Results and Performance Insights

- Reallocate budget from lower-performing channels (e.g., Discovery Plus Video) to higher-impact ones like FB Remarketing and Brand Search.
- Conduct tests on uncertain channels to refine performance insights.
- Enhance ROI by leveraging deeper audience segmentation.
- Maintain a diverse media mix to balance risk and reach.

---

**Note:** For further details or implementation guidance, please refer to the project repository.
