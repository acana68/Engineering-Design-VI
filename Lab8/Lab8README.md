# Lab 8 - Data Analysis

## Overview

This lab uses the system data collected from Lab 7 and performs data analysis using Python libraries such as NumPy, SciPy, Pandas, Matplotlib, scikit-learn, and Keras. The analysis includes visualizations like histograms, box plots, and regression predictions.

## Installations

Required libraries were installed using:

```
pip install -U numpy scipy scikit-learn matplotlib pandas keras
```

## File Setup

Downloaded and copied the scripts needed for analysis:

![lab8#1](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab8/lab8%231.png?raw=true)

Moved the `cpudata.csv` file to the working directory:

![lab8#2](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab8/lab8%232.png?raw=true)

## Edits Made

Edited `plt_final.py` to use memory data instead of temperature:

![nano_plt_final](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab8/nano_plt_final.png?raw=true)

Edited `plt_cv2.py` to match the data columns for regression:

![nano_plt_cv2](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab8/nano_plt_cv2.png?raw=true)

## Running the Scripts

Ran both plotting and regression scripts using:

```
python plt_final.py
python plt_cv2.py
```

Terminal output from running the scripts:

![lab8#3](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab8/lab8%233.png?raw=true)

## Output Graphs

### Time Series Plot

![lab8#4](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab8/lab8%234.png?raw=true)

### CPU Usage Histogram

![lab8#5](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab8/lab8%235.png?raw=true)

### Memory Available Histogram

![lab8#6](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab8/lab8%236.png?raw=true)

### CPU Box Plot

![lab8#7](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab8/lab8%237.png?raw=true)

### Memory Box Plot

![lab8#8](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab8/lab8%238.png?raw=true)

## Regression Output

Regression scatter plot with predictions:

![lab8#9](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab8/lab8%239.png?raw=true)

Final prediction and R² score from `plt_cv2.py`:

![lab8#10](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab8/lab8%2310.png?raw=true)
