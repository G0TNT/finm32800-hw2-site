# Dataframe: `hw2:fed_funds_futures` - 30-Day Fed Funds Futures (ZQ)

Daily bars from the CME Globex dataset (GLBX.MDP3), pulled with the ohlcv-1d schema and the parent symbol ZQ.FUT, which returns every listed ZQ contract. Columns: date, symbol, open, high, low, close, volume. A contract settles at 100 minus the average effective fed funds rate over its month, so 100 - close is the market's forecast of that average rate. The data includes calendar spreads such as ZQU6-ZQZ6 alongside the outright monthly contracts (ZQU6); filter them out with fedwatch.filter_outright_contracts before using prices as rate forecasts. Thinly traded months far from expiry may have no bar on a given day.


## DataFrame Glimpse

```
Rows: 11721
Columns: 7
$ date   <datetime[ns]> 2026-10-26 00:00:00
$ symbol          <str> 'ZQZ6'
$ open            <f64> 95.96
$ high            <f64> 95.965
$ low             <f64> 95.94
$ close           <f64> 95.95
$ volume          <u64> 15157


```

## Dataframe Manifest

| Dataframe Name                 | 30-Day Fed Funds Futures (ZQ)                                                          |
|--------------------------------|--------------------------------------------------------------------------------------|
| Dataframe ID                   | [fed_funds_futures](../dataframes/hw2/fed_funds_futures.md)                                       |
| Sources                        | CME Group                                          |
| Providers                      | Databento                                        |
| Provider Links                 | https://databento.com/                                   |
| Tags                           | Futures, Monetary Policy, Fed Funds                                             |
| Access Types                   |                                       |
| How is data pulled?            | Databento Historical API via Python                                                   |
| Data available up to (min)     | 2026-10-26 00:00:00                                                             |
| Data available up to (max)     | 2026-10-26 00:00:00                                                             |
| Dataframe Path                 | C:\Users\cekim\Desktop\Education\(3) UChicago\(1) First-Year\(1) Fall Quarter\FINM 32800 - Data Pipelines for Quant Research\HW\hw2-G0TNT\_data\fed_funds_futures.parquet                                             |


**Linked Charts:**


- [hw2:fedwatch_latest_forecast](../../charts/hw2.fedwatch_latest_forecast.md)



## Pipeline Manifest

| Pipeline Name                   | HW 2: The Yield Curve and the Policy Path                       |
|---------------------------------|--------------------------------------------------------|
| Pipeline ID                     | [hw2](../../../index.md)              |
| Maintainer                      | Jeremiah Bejarano               |
| Contributors                    | Jeremiah Bejarano |
| Repository                     | https://github.com/hw-finm-32800/hw2                  |
| Pipeline Web Page               | <a href="file://C:/Users/cekim/Desktop/Education/(3) UChicago/(1) First-Year/(1) Fall Quarter/FINM 32800 - Data Pipelines for Quant Research/HW/hw2-G0TNT/docs/index.html">Pipeline Web Page      |
| Date of Last Code Update        | 2026-10-27 07:29:18           |
| OS Compatibility                | Windows, Linux, macOS |
| Linked Dataframes               |  [hw2:crsp_treasury_consolidated](../../dataframes/hw2/crsp_treasury_consolidated.md)<br>  [hw2:fed_yield_curve](../../dataframes/hw2/fed_yield_curve.md)<br>  [hw2:fed_funds_futures](../../dataframes/hw2/fed_funds_futures.md)<br>  |


**Build Commands:**
```
doit

```

