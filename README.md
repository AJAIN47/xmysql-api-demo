# XMysql Auto-Generated API

This repository documents the steps I followed to auto-generate an API for a MySQL database using **XMysql**.

## Tool Overview

- **Tool Used**: **XMysql** and **MySQL workbench**
- **Purpose**: XMysql enables you to create REST APIs for any MySQL database instantly, without writing API code manually.

## Steps to Generate the API

### 1. Prerequisites

Make sure you have the following set up:

- **Node.js**: Download and install Node.js if it’s not already installed on your machine.
- **MySQL Database**: Ensure MySQL is installed and running. You can download it from the [MySQL Downloads](https://dev.mysql.com/downloads/).

### 2. Install XMysql

Open a terminal (Command Prompt or any CLI) and run the following command to install **XMysql** globally:

**command** - npm install -g xmysql

**Set Up Your MySQL Database**
Open MySQL Workbench or any MySQL client you prefer.
Create a Database. For this example, I named it sampledb:

**query** - CREATE DATABASE sampledb;

**Then create a products Table in this database**
**Insert Sample Data into the products table:**

**Run XMysql to Generate API Endpoints**
Go back to your terminal and run the following command, replacing your_mysql_username and your_mysql_password with your actual MySQL login credentials:

**command** - xmysql -h localhost -u your_mysql_username -p your_mysql_password -d sampledb

Once XMysql is running, it will start a local server at **http://localhost:3000** and automatically generate API endpoints for your MySQL database.

**Open your web browser or an API client (like Postman).**

**To List All Products, go to**
GET http://localhost:3000/api/products

**To Add a New Product, Get a Product by ID, or explore other endpoints, use the following routes:**

POST http://localhost:3000/api/products - Add a new product
GET http://localhost:3000/api/products/:id - Retrieve a product by its ID

**Screenshots**
Since XMysql doesn’t generate separate code files, I have included three screenshots to document the process:

**Screenshot of XMysql Command Execution:** Shows how I started the XMysql server.
**Screenshot of Available API Endpoints:** Lists the generated API routes.
**Screenshot of a Sample API Request:** Demonstrates the data returned by some of the API endpoints.
**Screenshot of DB creation on workbench.** Demonstrates the creation of database and tables.



