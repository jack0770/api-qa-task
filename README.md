# API Automation Task (Postman Collection)

This repository contains an automated API test suite for the [Restful-API.dev](https://api.restful-api.dev/objects) public endpoints. 

## Overview
Instead of using Playwright/TypeScript, I have implemented this task using **Postman**. As I specialize in manual and semi-automated API testing, I wanted to demonstrate my proficiency in building stateful, automated collections with JavaScript assertions.

## Features
- **End-to-End Flow**: The collection creates an object, retrieves it by ID, and then deletes it.
- **Dynamic Variables**: Uses `collectionVariables` to pass the `objectId` between requests.
- **Automated Assertions**: Each request includes tests for status codes, response time, and data integrity.

## How to run this collection

1. **Download** the `.json` file from this repository.
2. **Open Postman** and click the **Import** button.
3. Select the downloaded file.
4. Once imported, click on the collection name and select **Run Collection**.
5. Alternatively, you can run it via **Newman** (CLI):
   ```bash
   newman run API_Task.postman_collection.json