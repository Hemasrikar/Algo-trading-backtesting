# Algo-trading-backtesting


---
### Formulas

| - | Formula |
|-------|-------|
|Average Relative Quoted Speed | $\text{AvgRQS}_m = \frac{1}{N_m} \sum_{t \in m}\frac{\text{ASK}_t - \text{BID}_t}{\text{Mid}_t}$ |
| Order Imbalance | $\text{OIB}_m = \sum V^{buy}_m - \sum V^{sell}_m$ |
| Average Depth Imbalance | $\text{AvgDepthImb}_m = \frac{1}{N_m} \sum_{t \in m} \frac{\text{ASKSIZ}_t - \text{BIDSIZ}_t} {\text{ASKSIZ}_t + \text{BIDSIZ}_t}$ |
| Traded Volume | $\text{Volume}_m = \sum_{t \in m} \text{SIZE}_t$ |
| One Minute return from Closing mid price | $r_m = \ln(\text{Mid}_{m}^{close}) - \ln(\text{Mid}_{m-1}^{close})$ |
| Realized Volatility | $\text{RV}_m = \sum_{i=m-59}^{m} r_i^2$ |


$Ret_{t+1}=\alpha+\beta_1OIB+\beta_2RelSpr_t+\beta_3Vol_t+\beta_4Volat_t+\varepsilon_{t+1}$