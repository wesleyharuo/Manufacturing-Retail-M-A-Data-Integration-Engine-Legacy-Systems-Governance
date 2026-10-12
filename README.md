# Manufacturing-Retail-M-A-Data-Integration-Engine-Legacy-Systems-Governance
Project Overview
Implementation of a robust middleware and ETL integration layer to unify legacy systems, enterprise resource planning platforms (such as SAP and Microsoft Dynamics 365 Business Central), and commercial front-ends, ensuring data integrity across sales, inventory, and finance.

Business Challenge
Retailers and manufacturing firms often operate with disconnected data silos, making unified business visibility difficult and causing discrepancies between billing records, physical inventory counts, and general ledger cash flows.

Technical Architecture & Implementation
Generic Integration Engine: Developed modular Python and SQL routines for extracting, transforming, and loading (ETL) data from disparate sources into a unified centralized repository.

Accounting & Operational Reconciliation: Automated cross-system reconciliation matching POS sales data, inventory adjustments, and General Ledger records.

Executive Business Intelligence: Built dimensional data models utilizing Star Schema design principles and developed advanced Power BI analytical reports for profit margin tracking, managerial income statements (P&L), and inventory turns.

To make it feel like a real platform the CIO’s team would use day to day, I set it in a believable scenario: Project Meridian, where Halvorsen Manufacturing (SAP) is absorbing Northgate Retail (Business Central), now on Day 142 of the integration. The numbers connect across the page, so the story holds up when someone looks closely:

The ETL success rate works out to 2,841 of 2,866 runs. The hourly chart shows those failures clustering in the 04:00–06:00 batch window.
Those failures trace back to the Business Central stock-sync timeout. It appears as the red, pulsing edge in the topology and as the top “Failed” row in the pipeline monitor.
That same failure explains why inventory accuracy sits below its 98.5% target. The weak material master score (79, missing units of measure) is the root cause called out under the data quality chart.
The $1.90M unreconciled total on the finance card is the sum of the six entity bars, with Northgate US carrying the largest share.
The governance alerts are specific to a Canadian deal: a SOX segregation-of-duties conflict, a Quebec Law 25 data-residency breach, and a PCI certificate about to expire on legacy POS.

Key Technologies Used
Languages & Data Engineering: Python, Pandas, Advanced SQL

ERP & Systems: SAP, Microsoft Dynamics 365 Business Central

BI & Modeling: Power BI, DAX, Star Schema modeling

Results and Impact
Guaranteed strict data consistency between shop floors/retail stores and the financial directorate.

Cut audit preparation and monthly accounting close times down significantly.

Empowered leadership to make data-driven decisions backed by real-time financial and operational metrics.


<img width="2880" height="4752" alt="Integration Command Center@2x" src="https://github.com/user-attachments/assets/12602996-dbaf-4d50-bae9-27fbffb9ae06" />



