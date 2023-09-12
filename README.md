# Time-series-window-resampling
Python code. Window resampling technique to extract rows/examples that match individual pieces of the serie with length defined as window length. Therefore, a dataset is obtained with more examples and less columns (its number is equal to window), as we could think of this thechnique as a mini time series generator from original one


Welcome to the Time Series Windowing module of Python Magic Adventure! 🕰✨

Table of Contents
Introduction
Installation
Usage
Features
Contributing
License
Introduction
In the mystical land of Python Magic Adventure, there lies a powerful tool known as the "Time Series Windowing" module. This module allows you to manipulate time series data with ease, as if you were a wizard casting spells to reveal hidden patterns in the fabric of time itself.

Installation
To unlock the secrets of time series windowing, follow these simple steps:

Clone this repository to your local machine:

shell
Copy code
git clone https://github.com/your-username/python-magic-adventure.git
Install the required dependencies:

shell
Copy code
pip install -r requirements.txt
Import the TSWindow class from the magic_adventure.py script into your Python project:

python
Copy code
from magic_adventure import TSWindow
Usage
Once you've harnessed the power of the TSWindow class, you'll be able to slice and dice time series data with precision and control. Create windows, extract sets, and even visualize your data like a true time series wizard.

Here's a glimpse of what you can do:

python
Copy code
# Create a time series window with specific input size, gap, and label size
window = TSWindow(input_size=10, gap=2, label_size=5)

# Extract time series sets
X_window, y_window, _ = window.extract_sets(data)

# Visualize the time series splits
window.plot_splits(data, X_window, y_window, batch=0, feature=0)
Features
Time Series Windowing: Slice and dice time series data effortlessly.
Customization: Define input size, gap, and label size to suit your needs.
Visualization: Visualize your time series splits and label points with ease.
Flexibility: Extract sets for further analysis or machine learning tasks.
Contributing
The Time Series Windowing module is constantly evolving, and we welcome contributions from time series enthusiasts and data wizards alike. Whether you want to enhance the visualization capabilities or add new features, your contributions are valuable.

Please check out our contribution guidelines for more details.

License
The Time Series Windowing module is licensed under the MIT License. Feel free to use, modify, and share this magical tool as you embark on your time series adventures.

Unleash the power of time manipulation and uncover the mysteries hidden within your time series data! ⏳🔮






