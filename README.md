# TVIS3 Shiny App
<p align="right">
  <img src="https://github.com/Padhraig/TVIS3/blob/main/Screenshot%202025-02-26%20151625.png" width="150">
</p>
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)         
[![R Shiny](https://img.shields.io/badge/Built%20With-R%20Shiny-blue)](https://shiny.rstudio.com/)  
[![GitHub repo size](https://img.shields.io/github/repo-size/Padhraig/TVIS3)](https://github.com/Padhraig/TVIS3)  
[![GitHub last commit](https://img.shields.io/github/last-commit/Padhraig/TVIS3)](https://github.com/Padhraig/TVIS3)

## **🔬 Overview**  
**TVIS3** is a Shiny application for analyzing Type VI Secretion Systems in bacterial genomes. It integrates multiple bioinformatics tools into an interactive graphical interface. The tools selected were chosen based on a pre-determined pipeline, created by Amy J. G. Anderson et al (2023), entitled 'Distribution and diversity of type VI secretion system clusters in Enterobacter bugandensis and Enterobacter cloacae '.

---

What This App Does
Type VI Secretion Systems Suite offers several features for bioinformatics analysis, including:

## **🚀 Features**
✔ **DeepSecE Prediction** – Predict secretion systems using deep learning.  
✔ **SecRet6** – Identify T6SS components via BLASTp or HMMsearch.  
✔ **cblaster GUI** – Search homologous gene clusters.  
✔ **FastTree** – Construct phylogenetic trees.  
✔ **DeepTMHMM** – Predict transmembrane helices.  
✔ **HMMER** – Build and search hidden Markov models. 

---

Below is an example workflow overview outlining where some of these tools were used, and how for E. bugandensis

![Workflow Overview](https://github.com/Padhraig/TVIS3/blob/main/Screenshot%202025-02-26%20110722.png)

---

## **⚙️ Installation**
### **1️⃣ Install R & Required Packages**
Ensure you have **R (≥ 4.0.0)** installed. Then install dependencies:

```r
install.packages(c("shiny", "shinythemes", "shinyjs", "DT", "reticulate", "callr"))
```

### **2️⃣ Clone the Repository**
To download the app, use the following command:

```sh
git clone https://github.com/Padhraig/TVIS3.git
cd TVIS3
```

### **3️⃣ Running the App**
You can now run the Shiny app from the command line (Windows) or terminal (Linux and MacOS)

▶ Windows
Open Command Prompt (cmd) and run:

```sh
Rscript "C:/Users/yourusername/PATH To INSTALLATION/TVIS3-app.R"
```

▶ Linux / MacOS
Run the following command:

```sh
Rscript "/home/PATH To INSTALLATION/TVIS3-app.R"
```

---

⚡ Quick Launch as a Command
If you want to run the app without typing the full path every time, follow these steps:

🔹 Linux (Unix-based systems)
Make the script executable:
```sh
chmod +x TVIS3-app.R
```

Move it to a system-wide location:
```sh
sudo mv TVIS3-app.R /usr/local/bin/tvis3
```

Now, you can run the app simply by typing:
```sh
tvis3
```

🔹 Windows
Create a batch file (tvis3.bat):
Open Notepad, paste the following
```sh
@echo off
Rscript "C:/Users/yourusername/PATH To INSTALLATION/TVIS3-app.R"
```
Save it as tvis3.bat in a directory that is in your system PATH (e.g., C:\Windows\System32).

Now, you can launch the app by typing:
```sh
tvis3
```

Dependencies
TVIS3 integrates multiple bioinformatics tools. Ensure these dependencies are installed before running the app:
---

| Tool         | Description                                         | Installation Link |
|-------------|-----------------------------------------------------|------------------|
| **R** (≥ 4.0.0) | Required for running the Shiny app            | [Download R](https://cran.r-project.org/) |
| **Conda**      | Used for managing Python environments           | [Install Conda](https://www.anaconda.com/download) |
| **DeepSecE**   | Predicts secretion systems using deep learning  | [DeepSecE GitHub](https://github.com/zhangyumeng1sjtu/DeepSecE/blob/main/README.md) |
| **SecRet6**    | Identifies T6SS components using BLASTp or HMMsearch | [SecRet6 Webpage](https://bioinfo-mml.sjtu.edu.cn/SecReT6/t6ss_prediction.php) |
| **cblaster**   | Searches homologous gene clusters              | [cblaster GitHub](https://github.com/gamcil/cblaster/blob/master/README.md) |
| **FastTree**   | Constructs phylogenetic trees                  | [FastTree PDF](https://morgannprice.github.io/fasttree/) |
| **DeepTMHMM**  | Predicts transmembrane helices                 | [DeepTMHMM Webpage](https://dtu.biolib.com/DeepTMHMM) |
| **HMMER**      | Builds and searches hidden Markov models       | [HMMER GitHub](https://github.com/EddyRivasLab/hmmer/blob/master/README.md) |

---

🛠 Troubleshooting
"Rscript is not recognized" error?
→ Add R to your system PATH.

The app doesn't open?
→ Manually open the Listening on http://127.0.0.1:XXXX link in your browser.

❌ Other Issues?
Create a GitHub Issue in this repository, and describe your problem or email us at TVIS3.Help@gmail.com
