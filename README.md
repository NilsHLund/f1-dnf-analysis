# Formula 1 DNF Prediction

## Overview
This project aims to **analyze and model DNF (Did Not Finish) outcomes** in Formula 1 using historical race data.

---

## Dataset Description
This dataset contains **comprehensive historical Formula 1 data** curated specifically for DNF prediction.  
It spans **over seven decades** of racing and merges results, driver, constructor, and circuit data.

### Key Information:
- Each row represents a single driver’s race result.
- A **DNF** is represented by `target_finish = 0`, while finishing drivers have `target_finish = 1`.
- Features include:
  - **Race details:** `year`, `round`, `grid`, `laps`, `points`
  - **Driver info:** `driverRef`, `surname`, `dob`, `nationality_x`
  - **Constructor details:** `constructorRef`, `name`, `nationality_y`
  - **Circuit data:** `circuitRef`, `location`, `country`, `lat`, `lng`, `alt`
  - **Performance stats:** `positionOrder`, `fastestLap`, `fastestLapSpeed`
  - **Temporal fields:** `date`
  - **Target:** `target_finish`

## Data Types Summary

| # | Column | Non-Null Count | Dtype |
|---|---------|----------------|-------|
| 0 | resultId | 10000 | int64 |
| 1 | raceId | 10000 | int64 |
| 2 | year | 10000 | int64 |
| 3 | round | 10000 | int64 |
| 4 | grid | 10000 | int64 |
| 5 | positionOrder | 10000 | int64 |
| 6 | points | 9029 | float64 |
| 7 | laps | 9022 | float64 |
| 8 | milliseconds | 8982 | object |
| 9 | fastestLap | 10000 | object |
| 10 | rank | 10000 | object |
| 11 | fastestLapTime | 10000 | object |
| 12 | fastestLapSpeed | 9047 | object |
| 13 | driverRef | 10000 | object |
| 14 | surname | 10000 | object |
| 15 | forename | 10000 | object |
| 16 | dob | 10000 | object |
| 17 | nationality_x | 10000 | object |
| 18 | constructorRef | 10000 | object |
| 19 | name | 10000 | object |
| 20 | nationality_y | 10000 | object |
| 21 | circuitRef | 10000 | object |
| 22 | circuitId | 10000 | int64 |
| 23 | name_y | 10000 | object |
| 24 | location | 10000 | object |
| 25 | country | 10000 | object |
| 26 | lat | 10000 | float64 |
| 27 | lng | 10000 | float64 |
| 28 | alt | 10000 | int64 |
| 29 | date | 10000 | object |
| 30 | target_finish | 10000 | int64 |

**dtypes:**  
- `float64`: 4 columns  
- `int64`: 9 columns  
- `object`: 18 columns  

---