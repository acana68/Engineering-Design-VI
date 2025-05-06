# Lab 10: Blockchain

This lab demonstrates basic blockchain concepts such as hashing, mining, and running a decentralized application. I followed the instructions from Lesson 10 in the IoT GitHub repository and documented each step with screenshots.

---

## Step-by-Step Walkthrough with Explanations

### 1. Running the hash function
![step1](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab10/lab10%231.png?raw=true)  
I executed `hash_value.py` twice to show that the output changes each time. This demonstrates that the hash includes randomness (like a timestamp or salt).

---

### 2. Hashing using SHA-256
![step2](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab10/lab10%232.png?raw=true)  
I used Python’s `hashlib` library in the terminal to run a SHA-256 hash on a string. I also checked the digest size and block size to understand the structure of the hash.

---

### 3. Running a simple blockchain
![step3](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab10/lab10%233.png?raw=true)  
Next, I ran `snakecoin.py` which prints a minimal blockchain. Each block includes the index, proof, previous hash, and transactions.

---

### 4. Running the full blockchain server
![step4](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab10/lab10%234.png?raw=true)  
I tried to run `snakecoin-server-full-code.py` to start a web-based blockchain server. This server accepts transactions and allows mining.

---

### 5. Installing Flask to fix missing module
![step5](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab10/lab10%235.png?raw=true)  
An error occurred because Flask was not installed. I fixed it by running `pip install flask`.

---

### 6. Server running successfully
![step6](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab10/lab10%236.png?raw=true)  
After installing Flask, I successfully ran the blockchain server on port 5000.

---

### 7. Submitting a transaction via curl
![step7](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab10/lab10%237.png?raw=true)  
I used `curl` to post a new transaction to the server. This mimics a blockchain client sending data to the network.

---

### 8. Mining a new block
![step8](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab10/lab10%238.png?raw=true)  
Then I called the `/mine` endpoint to mine the block. The server created a new block and included the submitted transaction.

---

### 9. Cloning the second blockchain app
![step9](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab10/lab10%239.png?raw=true)  
I cloned the `python_blockchain_app` repo by Satwik Kansal, which contains a more advanced blockchain app with a web interface.

---

### 10. Checking for the folder
![step10](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab10/lab10%2310.png?raw=true)  
I had issues finding the folder after cloning. This was because I was looking in the wrong directory path.

---

### 11. Using `find` to locate the directory
![step11](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab10/lab10%2311.png?raw=true)  
I used the `find` command to search for the actual location of `python_blockchain_app`.

---

### 12. Navigating to the correct path
![step12](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab10/lab10%2312.png?raw=true)  
After locating the directory, I navigated to it using a relative path instead of assuming it was in the home directory.

---

### 13. Editing node_server.py
![step13](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab10/Lab10%2313.png?raw=true)  
I opened `node_server.py` and uncommented the final `app.run()` line so the Flask server would start correctly.

---

### 14. Web server running at 127.0.0.1:5000
![step14](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab10/lab10%2314.png?raw=true)  
After starting the app, I opened it in the browser. This is the homepage of the decentralized content-sharing web app.

---

### 15. Posting and mining content
![step15](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab10/lab10%2315.png?raw=true)  
I added a post with my name and clicked "Request to mine." The blockchain confirmed that "Block #1 is mined" and the post appeared on the page.

---

