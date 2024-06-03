---
id: Bank Data verification Service
title: Bank Data verification Service
description: 'Bank Data verification Service'
sidebar_position: 3
---
As the name suggests, the Bank Data Verification Service is all about banking data. On the one hand, the value-added service offers the worldwide possibility of checking business partner bank data qualitatively and formally and provides them with concrete information and suggestions for correction. The service represents the business-critical banking data attributes for 125 countries.
On the other hand, the service offers the possibility to verify a bank date on an ad hoc basis in order to obtain further bank data insights. As special ad on is, verification functionalities from tax compliance, compliance and the fight against fraud are implemented in the service. With this service, they are immediately proactively informed as soon as a known fraudulent bank data is in your system.

**Value Proposition**
![Bank Data verification](@site/static/img/value-proposition.png)

**How is the service related to BPDM?**
The database for this service consists of unique business partners with high address quality, up-to-date addresses and identifiers. However, in order to actually be able to do transactional business with your business partners, syntactically correct and error-free bank data is required. Thus, correct, error-free and non-fraudulent bank data contribute to the 360-degree view of business partners in the supply chain.

**What is the Output of the  Bank Data Verification Service?**

BDV has to validate the correctness of the IBAN number in all defined SEPA countries based on the rules defined by the European Payments Council for SEPA and the European Committee for Banking Standards (ECBS) for IBAN based on ISO 13616. The Bank Account Number contains the individual account number, the routing number and the SWIFT Code of the bank and the BDV has to verify the correctness of the Business Identifier Code (BIC/SWIFT) of Financial Institutions. BDV has to verify the correctness of the National Bank Account number as defined by the national bank institutions.
BDV with the support of the Fraud Prevention application has to verify if a bank account is affected by Fraud.  This verification has to include the information of the Fraud status and timeframe of affection.

## Out of Scope

The BDV product does not contain the functionality to correct and/or enrich a bank data record.
Bank Data Verification Dashboard
![Bank Data Verification Dashboard](@site/static/img/bpv-dashboard.png)

  Example Image illustration of an BDV dashboard could look like

BDV has to contain the following dashboard-based functionalities:

1. Visualization of CX Member bank data verification results
2. Various bank data filter functionalities based on the bank data model
3. BDV target setting
4. Bank data record target versus actuals
5. Bank data rule results supported by dashboard visualization capabilities
6. Bank data visualization by country type
7. BDV statistical report
8. Search function
9. BDV dashboard settings by time, KPI, layout and view, country, language limited to German and English

The results of BDV are accessible via a defined API and Changelog file managed via the Bank Data Sharing State Controller.

**Overview Components Architecture**
![Bank Data Verification Architecture](@site/static/img/bpv-architecture.png)
![BDV Dashboard Architectural Components](@site/static/img/bdv-dashboard-architecture-component.svg)
