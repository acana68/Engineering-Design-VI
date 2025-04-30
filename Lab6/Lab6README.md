# Lab 6 – Node.js and Pystache
The first step was confirming the installation of Node.js, npm, and Python.  
![lab6#1.png](https://github.com/your-username/your-repo/raw/main/lab6%231.png)  
Confirmed Node.js v22.15.0, npm v10.9.2, and Python 3.13.3 were installed successfully.  
This script creates a basic HTTP server that displays "Hello, World!" in the browser.  
```bash
node hello-world.js
```  
![lab6#2.png](https://github.com/your-username/your-repo/raw/main/lab6%232.png)  
The server started on port 3000.  
![lab6#3.png](https://github.com/your-username/your-repo/raw/main/lab6%233.png)  
Navigating to `127.0.0.1:3000` displayed the message "Hello, World!".  
This script also starts a server but logs request/response events to the console.  
```bash
node hello.js
```  
![lab6#4.png](https://github.com/your-username/your-repo/raw/main/lab6%234.png)  
Each time the browser refreshed, it printed log messages to the terminal.  
![lab6#5.png](https://github.com/your-username/your-repo/raw/main/lab6%235.png)  
The message "Hello World!" was displayed in the browser on port 8080.  
This server updates and tracks how many times the page has been refreshed.  
```bash
node http.js
```  
![lab6#6.png](https://github.com/your-username/your-repo/raw/main/lab6%236.png)  
The console displayed incrementing values each time the page was refreshed.  
![lab6#7.png](https://github.com/your-username/your-repo/raw/main/lab6%237.png)  
The browser output showed the current number of refreshes. This data was stored in `test.txt`.  
Pystache was installed using pip and used to render Mustache-style templates in Python.  
```bash
pip install pystache
```  
![lab6#8.png](https://github.com/your-username/your-repo/raw/main/lab6%238.png)  
Pystache installed successfully.  
This script demonstrates rendering of direct template strings, template files, and parsed templates.  
```bash
python say_hello.py
```  
![lab6#9.png](https://github.com/your-username/your-repo/raw/main/lab6%239.png)  
The output showed multiple template renderings including "Hi Alexa!", "Hello, World!", and parsed lines using data.

