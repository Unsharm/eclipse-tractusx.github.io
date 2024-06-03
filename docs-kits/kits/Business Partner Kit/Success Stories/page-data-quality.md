---
id: Data Quality Dashboard
title: Data Quality Dashboard
description: 'Data Quality Dashboard'
sidebar_position: 5
---
Data Quality Dashboard is a core function for profiling, measuring and evaluating one's own master data quality of Business Partner master data sets. In addition, fields of action are shown how a data defect can be rectified. On the other hand, it is also a way to control the own Business Partner data quality and control the data quality in the CX pool. In the Data Quality Dashboard  itself, no data are cleansed and this service belongs to Golden Record to measure and profile  the quality there. In the CX BPDM project, the conception, design and implementation ran under value-added services, but its belongs to core service golden record.
But DQD can do even more. It also measures and visualizes the LSA topic with regard to the degree of fulfillment/maturity of the LSA assignments. However, this service can also be used without anyone wanting to share, but would like to know what the in-house quality of business partners looks like. Especially against the background of harmonization or digitalization projects or implementation, migrations of business partner master data in the context of M&A activities.

## Value Proposition  

![Data Quality Dashboard](@site/static/img/dqd-value-proposition.png)

Whether it's customers or suppliers, poor master data quality can lead to quotes being misspelled, service employees being at the wrong address, or deliveries going to the wrong places. Therefore, it is increasingly important for the operations department that all company data is as accurate as possible. With the increase in data-based work, data analysis and data science use cases, the importance of data quality is also increasing.
Incorrect analysis or incorrect machine learning modeling quickly leads to wrong decisions being made. And this quickly costs money: Whether it's lower effects, wrong strategic decisions or incorrect monitoring of business processes – correctness is based on data quality. A company's image can also suffer greatly from poor data quality.
For example, if the quality of master data is low, incorrect product information may be communicated to the customer via the channels. This leads to confusion or frustration when you get different products than you expect. Another example is in the area of user experience. If customers expect a delivery and it is based on incorrect or outdated data, the customer will have a very bad experience.
While there are many internal processes that benefit greatly from high data quality, in the end it is the customer who always benefits. Whether it's more efficient or personalized channels, faster processing, better products or services, everything contributes to the fact that customers have an advantage.  
Therefore, data quality must not be considered in isolation for internal tasks, but must be thought through to the end of the process chain. Much of the information, whether master data or transaction data, ultimately has an impact on the channels and thus directly on the customer.

![DQD Value proposition](@site/static/img/value-proposition-data-quality.png)

How is the service related to BPDM?
Data Quality Dashboard is a core function for profiling, measuring and evaluating one's own master data quality of Business Partner master data sets. In addition, fields of action are shown how a data defect can be rectified. On the other hand, it is also a way to control the own Business Partner data quality and control the data quality in the CX pool. The Data Quality Dashboard (DQD) has to rely on a set of clearly defined quality rules which is the basis of the Golden Record Process and secure the syntactical and logical correctness of mission critical business partner data attributes. DQD has to capture at least 117 countries based on ISO 3166-1. DQD has to validate BP data records in the Inbound and Outbound Persistence of the related Catena-X (CX) Member who licensed DQD. Each DQD rule has to validate the syntactical correctness of defined mandatory, regulatory required and optional BP data record attributes related towards the specific regulations by the country authorized institutions. DQD has to visualize the outcome of the data quality rules via a dashboard.

What is the output of Data Quality Dashboard
The Data Quality Dashboard has to be a screening tool of the record process, rules, methodology and allocation of the BPN ID (Business Partner Number Identification) for Legal, Site and Address data records. DQD has to focus his validation and monitoring capabilities on all mandatory, regulatory required and optional business mission critical BP data record attributes to enable the CX Member to validate any impact on logistical, financially or communication relevant processes between the CX Member and his business partner. Furthermore, this transparency has to support the CX Member by improving his business partner related due diligence processes.  The Data Quality Dashboard has to contain the capability to store the outcome of DQD results and has to enable the definition of CX member specific data quality KPIs (Key Performance Indicator) and mapping against actual quality results.
Out of Scope
DQD rules have to be focused on the analysis of BP data record quality on a syntactical or content basis if possible. DQD does not focus on validating semantical correctness or data enrichment services. DQD does not contain the functionality to correct and/or enrich a BP data record, because this is part of the golden record process.
DQD Dashboard
![DQD Dashboard](@site/static/img/dqd-dashboard.png)

Example Image illustration of Data Quality Dashboard could look like

The DQD Dashboard provide the capabilities:

1. Visualization of Business Partner Data records as defined by the Golden Record Process based on the CX-0076.
2. DQD contains the visibility of BP data by user role and user based filter functions. The BP data can get filtered by:
1 Year, quarter or month
2 Country or Region
3 3. By BP type as customer or supplier
4.By BP data record type BPNL, BPNS or BPNA as defined
4 Visualization of Data Quality Screening results based on DQD KPIs and related achievements in percentage.
5 DQD is available in German and English language

## Overview Components Architecture

![DQD Architecture](@site/static/img/dqd-components-architecture.svg)
![DQD Architectural Components](@site/static/img/dqd-architectural-components.png)

DQD uses the Gate API CX-0074_V.1.1.0 or higher and the Pool API CX-0012_V.1.0.0 or higher for pulling BP data records. DQD is a client/ server cloud application which contains a Web Client and a Cloud Server Application. DQD has to contain a user and authorization management capability aligned with the CX Portal and Marketplace user management. DQD intend to support the EDC Asset function capability and has to be available in English and German language.
