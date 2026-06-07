# Professional Services Operations & Profitability Intelligence Platform

## Project Overview

This project transforms professional services project tracking data into a structured business intelligence platform.

The current development dataset is an Excel snapshot of MSD projects for 2025. The final target architecture is designed to support a refreshable pipeline from Google Sheets into PostgreSQL and Superset.

## Business Objective

The goal is to help management understand:

- Which projects generate revenue and profit
- Which sectors are most profitable
- Which sales channels produce better business
- Which engineers are overloaded
- Which projects are delayed or risky
- Which vendors/OEMs contribute to profitable delivery
- Which services should be expanded or reviewed

## Target Architecture

```text
Google Sheets / Excel Snapshot
        ↓
Raw Ingestion Layer
        ↓
Validation Layer
        ↓
Cleaning / Staging Layer
        ↓
Warehouse Star Schema
        ↓
Analytics Marts
        ↓
Superset Dashboards
        ↓
Executive Insights
