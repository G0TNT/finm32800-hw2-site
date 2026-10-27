# Dataframe: `hw2:crsp_treasury_consolidated` - CRSP Treasury Consolidated

Consolidated CRSP US Treasury database combining daily pricing data (prices, yields, durations) with issue-level characteristics (coupon, maturity, issue date). Sourced from WRDS.


## DataFrame Glimpse

```
Rows: 2530592
Columns: 20
$ kytreasno                  <f64> 200711.0
$ kycrspid                   <str> '19710215.205370'
$ tcusip                     <str> '912827AK'
$ caldt             <datetime[ns]> 1970-01-02 00:00:00
$ tdatdt            <datetime[ns]> 1967-08-30 00:00:00
$ tmatdt            <datetime[ns]> 1971-02-15 00:00:00
$ tfcaldt                    <i64> 0
$ tdbid                      <f64> 97.03125
$ tdask                      <f64> 97.15625
$ tdaccint                   <f64> 2.0448369565217
$ tdyld                      <f64> 0.00021825836291607
$ price                      <f64> 99.1385869565217
$ tcouprt                    <f64> 5.375
$ itype                      <f64> 2.0
$ original_maturity          <f64> 3.0
$ years_to_maturity          <f64> 1.0
$ tdduratn                   <f64> 394.45102379813
$ tdretnua                   <f64> 0.0012418439667652
$ days_to_maturity           <i64> 409
$ callable                  <bool> False


```

## Dataframe Manifest

| Dataframe Name                 | CRSP Treasury Consolidated                                                          |
|--------------------------------|--------------------------------------------------------------------------------------|
| Dataframe ID                   | [crsp_treasury_consolidated](../dataframes/hw2/crsp_treasury_consolidated.md)                                       |
| Sources                        | CRSP                                          |
| Providers                      | WRDS                                        |
| Provider Links                 | https://wrds-www.wharton.upenn.edu/                                   |
| Tags                           | Treasury, Fixed Income, Yield Curve                                             |
| Access Types                   |                                       |
| How is data pulled?            | WRDS via Python                                                   |
| Data available up to (min)     | N/A (large file)                                                             |
| Data available up to (max)     | N/A (large file)                                                             |
| Dataframe Path                 | C:\Users\cekim\Desktop\Education\(3) UChicago\(1) First-Year\(1) Fall Quarter\FINM 32800 - Data Pipelines for Quant Research\HW\hw2-G0TNT\_data\TFZ_consolidated.parquet                                             |


**Linked Charts:**

- None


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

