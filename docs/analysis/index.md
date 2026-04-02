# Analysis: System Overview

Welcome to the **StandCloud** analysis hub. This page provides a high-level summary of the platform's core modules, 
designed to help production managers, product owners, and QA specialists navigate the system's analytical capabilities.

---

## Global Production Dashboard
The primary entry point for monitoring the health of your manufacturing line. 
It provides real-time visibility into testing volumes and quality trends.

* **Key Metrics:** Monitor total test runs, pass/fail percentages, and average cycle times.
* **Trend Analysis:** Use the production history histogram to identify daily performance fluctuations.
* **Time Filtering:** Quickly toggle between daily, weekly, and monthly reports.

[Read more about the Dashboard](./home.md)

---

## Detailed Test Traceability
A deep-dive tool for investigating the specific lifecycle of an individual hardware unit. 
This section is critical for root-cause analysis of production failures.

* **Unit Metadata:** Access full hardware IDs, timestamps, and physical testing locations.
* **Hierarchical Test Plans:** Review the status of every sub-test (e.g., Temperature, Humidity) within a complex test run.
* **Diagnostic Logs:** View real-time messages and error codes from the test stand to distinguish between product defects and setup issues.

[Read more about Detailed analysis](./test_run.md)

---

## Test Stand Infrastructure
Manage and monitor the physical hardware assets that power your testing environment. 
**StandCloud** ensures your infrastructure is as reliable as the products it tests.

* **Stand Inventory:** View all active testing stations, their hardware IDs, and physical locations.
* **Maintenance Logs:** Track the service history of each stand, including PSU replacements and calibration passes.
* **Connectivity:** Manage secure API keys required for hardware-to-cloud data transmission.
* **Station Performance:** Access dedicated dashboards for individual stands to identify equipment-specific bottlenecks.

[Read more about Test stands](./test_stands.md)
