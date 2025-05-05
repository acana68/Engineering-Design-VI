
# Lab 8 - Data Analysis

## Overview

This lab analyzes system data from Lab 7 using Python libraries: NumPy, SciPy, Matplotlib, Pandas, scikit-learn, and Keras. The data is visualized through time series, histograms, box plots, and regression analysis.

## Installations

```
pip install -U numpy scipy scikit-learn matplotlib pandas keras
```

## File Setup

Copied scripts using:

```
cp ~/iot/*8/plt_final.py .
cp ~/iot/*8/plt_cv2.py .
```

## Edits

Updated `plt_final.py` to use `Memory Available GB` instead of temperature.  
![plt_final.py](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab8/nano_plt_final.png?raw=true)

Modified `plt_cv2.py` for prediction and regression.  
![plt_cv2.py](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab8/nano_plt_cv2.png?raw=true)

## Run

Moved the CSV file:

```
move "%USERPROFILE%\Downloads\cpudata.csv" "%USERPROFILE%\cpudata.csv"
```

Ran the scripts:

```
python plt_final.py
python plt_cv2.py
```

## Results

### Time Series  
![lab8#1](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab8/lab8%231.png?raw=true)

### CPU Usage Histogram  
![lab8#2](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab8/lab8%232.png?raw=true)

### Memory Histogram  
![lab8#3](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab8/lab8%233.png?raw=true)

### CPU Box Plot  
![lab8#4](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab8/lab8%234.png?raw=true)

### Memory Box Plot  
![lab8#5](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab8/lab8%235.png?raw=true)

### Scatter Plot + Regression  
![lab8#6](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab8/lab8%236.png?raw=true)

### Terminal Output  
![lab8#7](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab8/lab8%237.png?raw=true)

### More Figures  
![lab8#8](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab8/lab8%238.png?raw=true)  
![lab8#9](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab8/lab8%239.png?raw=true)  
![lab8#10](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab8/lab8%2310.png?raw=true)
