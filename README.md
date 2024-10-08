# Boxing Metric Analysis

This project analyzes data from boxing matches and calculates a custom metric based on the types of punches landed by each fighter. The goal is to assign different weights to punches depending on their placement (head or body) and type (jab or power punch), thus creating a score that reflects the effectiveness of the fighter's punches.

## Project Description

The metric created in this project is based on the analysis of boxing matches, where points are awarded to fighters based on the punches they land. Different types of punches are assigned specific weights according to the placement of the punches (head or body). A higher score indicates more impactful punches landed by a fighter.

## Data Files

The project includes CSV files that store data from different boxing matches:
- `CaneloGGG2.csv`: Data from the Canelo vs. Golovkin fight (Canelo's victory).
- `joshuausyk.csv`: Data from the Joshua vs. Usyk fight (Usyk's victory).
- `JoshuaUsyk2.csv`: Data from the second Joshua vs. Usyk fight (Usyk's victory).
- `InoueButler.csv`: Data from the Inoue vs. Butler fight (Inoue's victory by knockout).

## Functionality

### `boxing_metric(data, fighter)`

This function calculates a score for a given fighter based on the punches they landed. It takes into account:
- **Punch types**:
  - Jab
  - Power punch
- **Punch placement**:
  - Head
  - Body

The function multiplies different combinations of punch types and placements by corresponding weights:
- Jabs to the head: 0.5 points
- Jabs to the body: 0.25 points
- Power punches to the head: 1 point
- Power punches to the body: 0.5 points

The total score represents the effectiveness of a fighter in landing impactful punches.

## Requirements

The project uses the following Python libraries:
- `pandas` for data manipulation.
- `plotly` for visualization (if visual output is intended).

To install the required libraries, you can run:

```bash
pip install pandas plotly
