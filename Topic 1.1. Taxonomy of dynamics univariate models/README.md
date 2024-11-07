# Dynamic-in-ts-linear-Model

```
# AR(1) and AR(2) Time Series Models

This project demonstrates the creation, analysis, and estimation of both stable AR(1) and unstable AR(2) time series models using Python. The stable AR(1) model captures a stationary time series with a first-order autoregressive process, while the unstable AR(2) model demonstrates a fluctuating, oscillating process with higher-order autoregressive dynamics.

The repository includes:
- Generation of stable and unstable time series using AR(1) and AR(2) models.
- Estimation of AR(1) and AR(2) models and analysis of their parameters.
- Stability checks for both models, ensuring proper model behavior.
- Diagnostic tests such as autocorrelation and residual analysis.
- Visualizations of the time series, autocorrelation functions (ACF), and model diagnostics.

## Contents
- **Stable AR(1) Model**: Code for generating a stable AR(1) time series and fitting an AR(1) model.
- **Unstable AR(2) Model**: Code for generating an unstable AR(2) time series and fitting an AR(2) model.
- **Stability Check**: Code to assess the stability of the AR(1) and AR(2) processes using the roots of the characteristic polynomials.
- **Model Estimation**: Estimation of AR(1) and AR(2) model parameters and evaluation of results.
- **Diagnostic Tests**: Includes residual diagnostics like autocorrelation, heteroskedasticity, and normality tests to assess the model fit.
- **Visualizations**: Plots of the generated time series, autocorrelation functions (ACF), and model diagnostics.

## Requirements

To run the code, you need Python 3.x and the following libraries:
- `numpy`
- `matplotlib`
- `statsmodels`

You can install the required libraries by running:
```
pip install numpy matplotlib statsmodels
```

## How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/ar1-ar2-time-series.git
   ```

2. Navigate to the project directory:
   ```bash
   cd ar1-ar2-time-series
   ```

3. Run the `generate_ar1_process.py` script to create the stable AR(1) time series and generate the plots:
   ```bash
   python generate_ar1_process.py
   ```

4. Run the `generate_ar2_process.py` script to create the unstable AR(2) time series and generate the plots:
   ```bash
   python generate_ar2_process.py
   ```

5. Run the `estimate_ar1_model.py` script to estimate the AR(1) model parameters and check its stability:
   ```bash
   python estimate_ar1_model.py
   ```

6. Run the `estimate_ar2_model.py` script to estimate the AR(2) model parameters and check its stability:
   ```bash
   python estimate_ar2_model.py
   ```

7. The output will include visualizations of the time series, ACF plots, and model diagnostics.

## Results and Discussion

- **Stable AR(1)**: The AR(1) model demonstrates a stationary process with a single autoregressive parameter. The estimation results highlight the stability of the model, with diagnostics confirming no significant autocorrelation in residuals and a good fit for short-term forecasting.
  
- **Unstable AR(2)**: The AR(2) model exhibits an unstable, oscillating process. The estimation captures the two autoregressive parameters, with results showing the characteristic diverging behavior. Residual diagnostics suggest the model fits the noisy data, but due to instability, it is not suitable for long-term forecasting.
