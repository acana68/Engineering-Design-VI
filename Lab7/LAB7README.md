# Lab 7 - CPU & Memory Logging with ThingSpeak and Google Sheets

## ThingSpeak Data Upload

I used the following command to run the ThingSpeak upload script:

![lab7-1](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab7/lab7%231.png?raw=true)

Below is the ThingSpeak chart output showing CPU usage and available memory:

![field1-field2chart](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab7/field1-field2chart.png?raw=true)

---

## Google Sheets Setup

I created a service account named `rpdata` and downloaded the credentials as a `.json` file:

![lab7-2](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab7/lab7%232.png?raw=true)

Here’s the service account key file:

![lab7-3](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab7/lab7%233.png?raw=true)

I copied the required files into my working directory:

![lab7-4](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab7/lab7%234.png?raw=true)

---

## Running Google Sheets Logger

I edited `cpu_spreadsheet.py` to include my sheet and key file names:

![lab7-5](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab7/lab7%235.png?raw=true)

Then I ran the script and began logging every 10 seconds:

![lab7-6](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab7/lab7%236.png?raw=true)

Logged data shows up in my Google Sheet:

![lab7-7](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab7/lab7%237.png?raw=true)

---

## Dependencies Installed

I installed the required libraries using pip:

![lab7-8](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab7/lab7%238.png?raw=true)

---

## Output During Live Logging

Below is the output showing periodic data entries and confirmation responses:

![lab7-9](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab7/lab7%239.png?raw=true)
