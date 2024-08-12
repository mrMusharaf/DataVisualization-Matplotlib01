### Data Visualization Using Matplotlib

**Overview**

This repository provides a series of Python scripts demonstrating how to visualizesimple salary data for Machine Learning Engineers, Data Scientists, and Computer Vision beginners using Matplotlib. The code snippets explore various Matplotlib features, including plot styling, labeling, adding legends, and using different visual themes.

**Table of Contents**

- [Introduction]
- [Features]
- [Installation]
- [Usage]
- [Examples]
- [Available Plot Styles]
- [Contributing]
- [License]

**Introduction**

This project is designed to help you get started with Matplotlib by providing practical examples of how to create professional-looking plots. You'll learn how to visualize salary trends across different roles in the tech industry, customize your plots with various styles, and save your visualizations for presentations or reports.

**Features**

- **Basic Plotting**: Create simple line plots to visualize data trends.
- **Custom Labels and Titles**: Add meaningful titles and axis labels to your plots.
- **Legends**: Distinguish between different data series using legends.
- **Custom Plot Styles**: Apply various Matplotlib styles, including `ggplot`, `seaborn`, and `xkcd`.
- **Save Plots**: Export your visualizations as PNG files for easy sharing.
- **Grid and Padding Adjustments**: Enhance plot readability with grids and automatic layout adjustments.

**Installation**
To run the code in this repository, you need to have Python installed along with the Matplotlib library.

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/salary-visualization-matplotlib.git
   ```
2. Install the required dependencies:
   ```bash
   pip install matplotlib
   ```

**Usage**

Each script in this repository demonstrates different aspects of Matplotlib. You can run any of the scripts to generate the corresponding plots.

For example, to generate a plot with custom styles and legends:

```bash
python plot_data.py
```

This will create a plot visualizing the median salary for ML Engineers, Data Scientists, and CV Experts by age.

**Examples**

**Basic Plotting**

```python
from matplotlib import pyplot as plt

x = [25, 26, 27, 28, 29, 30]
y = [33100, 33895, 34500, 35000, 36300, 36400]
py_y = [33000, 33200, 33400, 33500, 34000, 35000]

plt.plot(x, y)
plt.plot(x, py_y)
plt.show()
```

**Plot with Titles and Labels**

```python
plt.title('ML Engineers and Data Scientists Median Salary (PKR) by Age')
plt.xlabel("Age")
plt.ylabel("Median Salary (PKR)")
plt.plot(x, y, label='ML Engineers')
plt.plot(x, py_y, label="Data Scientists")
plt.legend()
plt.show()
```

**Advanced Plotting with Styles**

```python
plt.style.use('ggplot')
plt.plot(x, y, color='b', linestyle='--', linewidth=3, marker='o', label='ML Engineers')
plt.plot(x, py_y, color='g', linestyle='-', linewidth=2, marker='|', label="Data Scientists")
plt.legend()
plt.tight_layout()
plt.show()
```

**Available Plot Styles**

Matplotlib offers various pre-defined styles that can be easily applied to your plots. Some of the styles used in this repository include:

- `ggplot`
- `seaborn-v0_8`
- `_mpl-gallery-nogrid`
- `xkcd`

You can explore all available styles using:
**python**
print(plt.style.available)


**Contributing**

Contributions are welcome! If you have suggestions or improvements, feel free to open an issue or submit a pull request. Please ensure your code follows the existing style and is well-documented.

**License**

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
