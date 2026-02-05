# Algo-trading-backtesting


---
### Formulas

<table>
  <tr>
    <th>-</th>
    <th>Formula</th>
  </tr>
  <tr>
    <td>Average Relative Quoted Speed</td>
    <td>$\text{AvgRQS}_{m} = \frac{1}{N_m} \sum_{t \in m}\frac{\text{ASK}_t - \text{BID}_t}{\text{Mid}_t}$</td>
  </tr>
  <tr>
    <td>Order Imbalance</td>
    <td>$\text{OIB}_m = \sum V^{buy}_m - \sum V^{sell}_m$</td>
  </tr>
  <tr>
    <td>Average Depth Imbalance</td>
    <td>$\text{AvgDepthImb}_m = \frac{1}{N_m} \sum_{t \in m} \frac{\text{ASKSIZ}_t - \text{BIDSIZ}_t}{\text{ASKSIZ}_t + \text{BIDSIZ}_t}$</td>
  </tr>
  <tr>
    <td>Traded Volume</td>
    <td>$\text{Volume}_m = \sum_{t \in m} \text{SIZE}_t$</td>
  </tr>
  <tr>
    <td>One Minute Return</td>
    <td>$r_m = \ln(\text{Mid}_{m}^{close}) - \ln(\text{Mid}_{m-1}^{close})$</td>
  </tr>
  <tr>
    <td>Realized Volatility</td>
    <td>$\text{RV}_m = \sum_{i=m-59}^{m} r_i^2$</td>
  </tr>
</table>


$Ret_{t+1}=\alpha+\beta_1OIB+\beta_2RelSpr_t+\beta_3Vol_t+\beta_4Volat_t+\varepsilon_{t+1}$