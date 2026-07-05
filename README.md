# SOC Arsenal - User Documentation & Setup Guide

**SOC Arsenal** is a highly protected, portable, and offline-first assistant built for Security Operations Center (SOC) analysts. It uses local AI models and Threat Intel APIs to automate log parsing, threat intelligence gathering, and incident report generation.

---

## 🚀 1. Installation & First-Time Setup 
 

**Step 1: Extract the Application**
Extract the `SOC_Arsenal_Secure.zip` file to any folder on your computer (e.g., your Desktop or Documents).

**Step 2: Install Python**
Open terminal on same Path and run .\setup.bat

* *Note: This process takes 1-3 minutes and requires an internet connection just for this first setup.*

---

## ⚙️ 2. Running the Application 

**Step 1: Launch the Program**
Double-click the **`SOC_Arsenal.bat`** file.

**Step 2: First-Time Initialization (Automatic)**
* The first time you run the script, a black terminal window will appear. 


**Step 3: The System Tray**
Once the setup is complete, the program will run silently in the background. Look for the **Shield Icon (SOC Arsenal)** in your Windows System Tray (bottom right corner, near the clock).

---

## 🔑 3. Configuring API Keys 
To use the "Threat Intel" feature to check IPs and Domains, you need to add your API keys:
1. **Right-click** the SOC Arsenal Shield Icon in the System Tray.
2. Select **API Keys**.
3. A settings window will open. Paste your keys for VirusTotal, AbuseIPDB, etc.
4. Click Save. The keys are securely stored locally on your machine.

---

## 🎯 4. How to Use 

The core philosophy of SOC Arsenal is that it integrates into your workflow without making you switch windows.

1. **Highlight Text:** Highlight any raw log, IP address, or text you want to analyze in your SIEM, Terminal, or Browser.
2. **Press `Ctrl + Shift + X`:** The magical circular "Pie Menu" will appear right where your mouse is.
3. **Choose an Action:**
   * 📝 **Generate Report:** Turns messy logs into a clean, professional incident report.
   * ➕ **Add to Report:** Merges new findings into the report you are currently working on.
   * 🔍 **Threat Intel:** Takes the highlighted IP/Domain and checks it against all your configured APIs instantly.
   * 🧹 **Parse Logs:** Cleans up messy JSON or raw firewall logs into a readable summary.

*(Features like Bulk Scan, Email Analysis, and Report by CSV are currently disabled/in development).*

---
**Security Note:** 
The core logic of this application is fully compiled and protected (using Native C binaries / `.pyd`). It is entirely safe from unauthorized modifications.
