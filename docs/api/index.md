# Public API Reference

The **StandCloud** [Public API](https://standcloud.everypin.io/integration/api/v1/docs) 
provides a secure, read-only interface for accessing your 
production data and testing results. 
This tool allows production managers, QA specialists, and product owners to programmatically extract analytics, 
integrate quality metrics into internal BI or ERP systems, and build custom automated reports.

## Authentication

All API requests must be authenticated using a valid **API Key**. 

* **Security:** The key should be passed in the request header as `X-API-KEY`.
* **Access Control:** The API is strictly read-only, ensuring that your production 
  records remain immutable and secure while allowing for data transparency.

[Learn how to manage API keys](./../get_started/index.md#3-connecting-your-hardware)

---

## Core Endpoints

The v1 API is focused on providing granular visibility into test executions and device history. 
All endpoints below utilize the **GET** method.

### 1. Test Runs List
* **Endpoint:** `GET /test_run`
* **Purpose:** Retrieves a comprehensive list of all test sessions conducted within the organization.
* **Business Value:** This is the primary tool for production managers to aggregate historical data. 
  It allows for the extraction of large datasets to analyze production throughput over specific shifts, weeks, or months.

### 2. Detailed Test Run Analysis
* **Endpoint:** `GET /test_run/{test_run_id}`
* **Purpose:** Fetches exhaustive details about a specific test session using its unique identifier.
* **Business Value:** Ensures full traceability for auditing. It provides the metadata of the stand used, 
  exact start/end timestamps, and the final result, which is essential for verifying the testing conditions of a specific unit.

### 3. Failure Diagnostics
* **Endpoint:** `GET /test_run/{test_run_id}/failed_case`
* **Purpose:** Returns a targeted list of only the steps (test cases) that resulted in a `Fail` status within a specific run.
* **Business Value:** A critical tool for QA specialists. Instead of parsing thousands of lines of successful logs, 
  this endpoint allows for the immediate extraction of error logs and diagnostic messages to understand exactly why 
  a unit was rejected (e.g., failure in thermal cycling or insulation breakdown).

### 4. Device History (DUT)
* **Endpoint:** `GET /tested_dut`
* **Purpose:** Provides data focused on the physical devices under test (DUT).
* **Business Value:** Allows Product Owners to evaluate statistics from the perspective of specific serial numbers or part numbers. 
  This is useful for identifying "problematic" batches or generating a digital "Quality Passport" for every unit shipped to a customer.

---

## Interactive Documentation

For a full list of query parameters (such as limits, offsets, and filters) and to test these requests in real-time, 
please refer to our Swagger UI:

https://standcloud.everypin.io/integration/api/v1/docs
