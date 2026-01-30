# Biometric-Fusion-Avionics
An R Shiny-based framework for pilot workload monitoring using multi-modal biometric fusion and Machine Learning

[![R-Shiny](https://img.shields.io/badge/Tools-R%20Shiny-blue.svg)](https://shiny.rstudio.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Status](https://img.shields.io/badge/Status-Academic--Prototype-green.svg)]()

This repository contains the source code for an intelligent cockpit monitoring and adaptive intervention system. The project leverages machine learning to predict pilot cognitive states by fusing multiple biometric data streams, providing a "Digital Twin" approach for modern aviation safety.

## 🚀 Overview
Modern flight missions impose high cognitive demands on pilots. This framework addresses this challenge by:
1.  **Monitoring:** Real-time acquisition of 5 key metrics (Heart Rate, GSR, EEG Beta/Alpha, Blink Rate, and Interaction Latency).
2.  **Classification:** Using a **Random Forest** algorithm to categorize workload into Normal, Elevated, and Critical states (Achieved **94% accuracy** in simulations).
3.  **Adaptation:** Automatically reconfiguring the avionics interface and triggering autonomous assistance when critical stress is detected.

## 🛠 Features
- **Live Biometric Fusion:** Integrated processing of physiological and behavioral data.
- **XAI (Explainable AI):** Built-in "Variable Importance" analysis to understand model decision-making.
- **High-Resolution Export:** Capability to export analytical plots (Radar Charts, Importance Plots) in **600 DPI** for academic publications.
- **Interactive Dashboard:** Developed with **R Shiny** for a user-friendly simulation environment.

## 📂 Repository Structure
- `app.R`: The complete single-file Shiny application.
- `README.md`: Project documentation and setup guide.
- `figures/`: (Optional) Sample output plots from the system.

## 💻 Installation & Usage
1.  **Requirements:** Ensure you have [R](https://www.r-project.org/) and [RStudio](https://rstudio.com/) installed.
2.  **Install Libraries:**
    ```R
    install.packages(c("shiny", "shinydashboard", "ggplot2", "randomForest", "tidyr"))
    ```
3.  **Run the App:**
    Open `app.R` in RStudio and click **"Run App"** or execute:
    ```R
    shiny::runApp()
    ```

## 📊 Scientific Methodology
The system architecture follows a closed-loop logic:
- **Data Input:** Simulated via real-time sliders in the dashboard.
- **Processing:** Feature importance and probability estimation using Random Forest.
- **Output:** Dynamic adaptation messages and biometric radar profiling.

## 🎓 Citation & Acknowledgements
If you find this work useful for your research, please cite:
> **Çakır, M. (2026).** *A Multi-Modal Biometric Fusion Framework for AI-Driven Adaptive Avionics and Pilot Workload Mitigation.*

Special thanks to **Gemini (Google AI)** for technical assistance in R Shiny optimization and linguistic refinement of the documentation.

## 📄 License
Distributed under the MIT License. See `LICENSE` for more information.

---
**Contact:** [Mustafa Çakır (mustafa.cakir@iste.edu.tr)] - [Iskenderun Technical University/www.iste.edu.tr/person/mustafa-cakir]
