# TSWindow - Time Series Windowing

![Python Magic Adventure Logo](https://github.com/Marlup/Time-series-window-resampling/data/example-time-series-windowing.png)

Welcome to the Time Series Windowing module! 🕰✨

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Class Methods](#class-methods)
- [Contributions](#contributions)
- [License](#license)
<!--- [Contributing](#contributing)-->

## Introduction

<p style="text-align: justify; background-color: yellow; display: inline-block;">The TSWindow class is a Python module for time series data processing. It provides functionality for creating sliding windows on time series data to prepare it for machine learning tasks like forecasting. This README file provides an overview of the class and its key functionalities.
</p>

## Features

* Create sliding windows for time series data.
* Handle even and remainder splits.
* Visualize the sliding window splits.

## Installation

You can install the required dependencies using pip:

  ```shell
  pip install numpy matplotlib
  ```

1. Clone this repository to your local machine:

  ```shell
  git clone https://github.com/your-username/python-magic-adventure.git
  ```

1. Install the required dependencies:

  ```shell
  pip install -r requirements.txt
  ```

1. Import the TSWindow class from the window.py script into your Python project:

  ```Python
  from window import TSWindow
  ```

## Usage

The example below slice time series data. Create windows, extract sets, and visualize your data.

Here's a glimpse of what you can do:

  ```Python
  import numpy as np
  from matplotlib import pyplot as plt
  from ts_window import TSWindow

  # Create an instance of TSWindow (a window) with specific input size, gap, and label size
  window = TSWindow(input_size=10, gap=2, label_size=5)

  # Load your time series data as a NumPy array
  data = np.load("your_time_series_data.npy")

  # Extract time series sets
  X_window, y_window, _ = window.extract_sets(data)
  
  # Visualize the time series splits
  window.plot_splits(data, X_window, y_window, batch=0, feature=0)
  plt.show()
  ```

## Class Methods

`__init__(input_size=1, gap=0, label_size=1)`

Constructor for the **TSWindow** class. Initializes the window parameters.

`extract_sets(data, splits_into_batch=True, return_indices=False)`

Extracts windowed data and labels from the input time series data.

* `data`: A 3D NumPy array representing the time series data.
* `splits_into_batch`: If **True**, splits the data into batches for machine learning. Default is **True**.
* `return_indices`: If **True**, returns the start indices of each window. Default is **False**.
`plot_splits(data, data_win, labels, batch=0, feature=0, figsize=(12, 6))`

Plots the sliding window splits of the time series data.

* `data`: The original time series data.
* `data_win`: The windowed data obtained using **extract_sets**.
* `labels`: The corresponding labels obtained using **extract_sets**.
* `batch`: The batch to visualize. Default is **0**.
* `feature`: The feature to visualize. Default is **0**.
* `figsize`: The figure size for the plot. Default is **(12, 6)**.

## Contributions

Contributions from time series enthusiasts and data wizards alike are welcomed. Whether you want to enhance the visualization capabilities or add new features, your contributions are valuable.

Please, note that there aren't any contribution guidelines yet.

## License

The Time Series Windowing module is licensed under the [MIT License](https://github.com/git/git-scm.com/blob/main/MIT-LICENSE.txt). Feel free to use, modify, and share this magical tool as you embark on your time series adventures.

## Acknowledgments

The **TSWindow** class was developed by @Marlup.
Please feel free to contribute to this project, report issues, or suggest improvements. Happy time series analysis!





