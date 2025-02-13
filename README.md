# IPL Data Analysis Project

This project is a data analysis of the Indian Premier League (IPL) cricket tournament. The data is collected from the IPL website and the analysis is done using Python and its libraries.

## Project Structure

- `dataset/`: Contains the dataset used for analysis.
- `ipl_data_analysis/`: Contains the Jupyter Notebook for data analysis.

## Getting Started

### Prerequisites

- Python 3.x
- Jupyter Notebook
- Required Python libraries: pandas, numpy, plotly

### Installation

1. Clone the repository:
   ```sh
   git clone <git remote add origin https://github.com/huzaifazz/ipl-data-analysis-project.git>
   ```
2. Navigate to the project directory:
   ```sh
   cd ipl_data_analysis_project
   ```
3. Install the required libraries:
   ```sh
   pip install pandas numpy plotly
   ```

### Running the Analysis

1. Open the Jupyter Notebook:
   ```sh
   jupyter notebook ipl_data_analysis/ipl_data_analysis.ipynb
   ```
2. Run the cells in the notebook to perform the analysis.

## Analysis Overview

### Import Libraries

The following libraries are imported for data analysis:

```python
import pandas as pd
import numpy as np
import plotly.graph_objects as go
import plotly.express as px
```


### Load Dataset

The dataset is loaded using pandas:

data = pd.read_csv("ipl_dataset_2022.csv")
data


### Visualizations

* **Number of matches won by team in IPL 2022** :

  figure = px.bar(data, x=data["match_winner"], title="Number of Matches won in IPL 2022")
  figure.show()

  **Best Bowler in IPL 2022** :

  fig = px.bar(data, data["best_bowling"], title="Best Bowler in IPL 2022")
  fig.show()

## License

This project is licensed under the MIT License.

**Save this content in a file named `README.md` in t**he root directory of your repository.
