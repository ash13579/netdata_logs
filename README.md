# System Resource Monitoring with Netdata & Docker

This project demonstrates how to set up a real-time system and application performance monitoring dashboard using Netdata, run conveniently inside a Docker container.

---

## 📝 Project Overview

The objective of this task was to install and configure Netdata, a free and open-source monitoring tool, to visualize system-level metrics (CPU, memory, disk) and application-level metrics (specifically, Docker containers). The goal was to gain a practical understanding of how lightweight monitoring solutions can provide deep insights into a server or application's health and performance.

---

## 📊 Sample Dashboard Screenshot

Below is a screenshot of the live Netdata dashboard, the primary deliverable for this project. It showcases real-time monitoring of system resources.

![Netdata Dashboard](https://github.com/ash13579/netdata_logs/blob/main/metrics.png)



---

## 🛠️ Tools Used

* **Docker**: A platform to build, ship, and run applications in isolated environments called containers. Used here to run Netdata without a complex native installation.
* **Netdata**: A high-fidelity, real-time monitoring tool that auto-discovers and visualizes metrics from systems and applications.

---

## 🚀 Step-by-Step Guide

This section outlines the process followed to get the Netdata dashboard up and running.

### 1. Prerequisite: Install Docker

Before running Netdata, **Docker Desktop** was installed on the host machine (Windows/macOS/Linux) and confirmed to be running.

### 2. Run the Netdata Container

The core of the project was executing a single command in the terminal to download and run the official Netdata image:

```bash
docker run -d --name=netdata -p 19999:19999 netdata/netdata
