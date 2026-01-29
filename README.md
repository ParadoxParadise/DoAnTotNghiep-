# Distributed Smart SOC & Biometric Integration

**An integrated security monitoring solution for SMEs combining Network Security (SIEM) and Physical Security (Biometrics).**

## 📖 Overview
This project bridges the gap between digital and physical security. It deploys a **Distributed Security Operations Center (SOC)** using **Wazuh** for network monitoring and threat detection, integrated with a **Raspberry Pi-based Facial Recognition system**.

The system aims to provide a unified dashboard where security administrators can monitor network anomalies (e.g., brute force attacks) alongside physical access logs (e.g., unauthorized entry attempts).

## 🏗️ System Architecture
* **Core Core:** Wazuh Manager (hosted on Linux Server).
* **Edge Node:** Raspberry Pi 4 (acting as a Wazuh Agent & Biometric Scanner).
* **Integration:** Custom Python scripts bridging OpenCV data with Wazuh logs.

## 🚀 Key Features
* **Centralized SIEM:** Real-time log analysis and intrusion detection using Wazuh.
* **Biometric Physical Security:** Facial recognition system deployed on Raspberry Pi using OpenCV.
* **Unified Alerting:** Physical security events (e.g., "Unknown Face Detected") are sent to the Wazuh dashboard as security alerts.
* **Automated Response:** Configured active responses to block IP addresses or trigger alarms upon specific threat signatures.

## 🛠️ Tech Stack
* **SIEM:** Wazuh (Manager/Agent)
* **Hardware:** Raspberry Pi 4
* **Languages:** Python 3, Bash Scripting
* **OS:** Ubuntu Server, Raspberry Pi OS
* **Libraries:** OpenCV, face_recognition, requests
