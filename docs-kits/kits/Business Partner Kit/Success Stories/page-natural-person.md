---
id: Natural Person Screening Service
title: Natural Person Screening Service
description: 'Natural Person Screening Service'
sidebar_position: 4
---
The Natural Person Screening is a screening tool and methodology  to identify automated with a high probability if a BP data record in the Inbound Persistence is a Natural Person or a Legal Entity. The results of the validation is provided via a dashboard. NPS is a Value Added Services (VAS) application for Data Provider and Consumer to screen all BP data records in the own Inbound Persistence to find a Natural Person data record. NPS is based on an exclusion methodology. NPS visualize the outcome of the rules via a dashboard.

## Value Proposition

![Natural person screening service](@site/static/img/nps-benefits.png)

 How is the service related to BPDM?
The NPS service generally includes two objective aspects:

1. The first aspect is to use a set of different rules to recognize that a business partner master record is a natural person and thus stop further processing in the golden record process. This is due to the fact that no natural persons are to be stored in the CX pool.
2. The NPS Service – like other VAS services – provides a further building block for obtaining a 360-degree view of Business Partners in the sense of Know Your Business Partner, its classification and supports compliance with the General Data Protection Regulation when dealing with natural persons.
What is the Output/outcome of Natural Person Screenings ?
NPS contains a screening capability and a user interface which enables that no Natural Person data record will get passed into the Golden Record Process as the process handles solely Legal Entity data records.
The Natural Person Screening Dashboard (NPS) relies on a set of clearly defined screening rules which are the basis the validate if a Business Partner (BP) is a Natural Person or a Legal Entity. NPS captures at least 117 countries based on ISO 3166-1. NPS validates BP data records in the own Inbound Persistence of the related CX Member who licensed NPS. Each NPS rule  validates defined attributes of the BP data record via a specific rule set. The outcome of the main NPS rule methodologies are described below:
Identifier Check
NPS validates if the BP data record in the own Inbound Persistence is already a valid Golden Record data record with a valid BPN ID.
Locality Check
NPS validates the locality of the BP data record as a basis for further screening methodologies.
 Identification Check
NPS validates the given Identifier about their formal correctness and use the content of the Identifier via the NPS rule set to identify a Legal or a Non-Legal Entity.

Check via External Data Sources
NPS match BP data entries with appropriate global data sources to identify Natural Persons or Legal Entities.
Legal Form Check
NPS validates any Legal Form indicators of the BP data record against country specific company and institutional valid organizational forms.

Final Natural Person Identifier Check
NPS validates the BP data records against Natural Person Identifiers on a global basis.
Out of Scope
Natural Person Service does not contain the functionality to correct and/or enrich a BP data record.This is the task / target of BPDM Golden Record.

### NPS Dashboard

![Natural Person Screening Dashboard](@site/static/img/nps-dashboard.png)

Example Image illustration of NPS Dashboard could look like

The NPS Dashboard provide the following results:
Visualization of BP data records based on defined NPS screening methodologies:
Filter capabilities of BP data results

1. By time (year, quarter, month) for the duration of up to 3 years into the past
2. By NPS validation classification (Natural Person, Legal Entity, Undefined)
3. By Country
4. By Error Code Status (Red, Yellow, Green)
5. BP Data record detailed with NPS rule results
6. Number of rules used
7. Search function and scrollbars
8. Number of data records validated by NPS

Overview Components Architecture
![NPS Components Architecture](@site/static/img/nps-architecture.png)
