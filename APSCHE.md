# ServiceNow IT Incident Management System

## Project Overview
This project demonstrates the configuration and administration of a ServiceNow instance to optimize the IT Service Management (ITSM) lifecycle. The goal is to automate incident creation, categorization, assignment, and resolution pathways to reduce Mean Time to Resolution (MTTR).

## Core Configurations & Features Built
*   **User & Role Administration:** Configured custom IT Service Desk groups, user profiles, and Access Control Lists (ACLs) to secure data.
*   **Automated Assignment Rules:** Created routing rules that automatically assign incoming critical database or network incidents to the respective tier-2 support teams.
*   **Service Level Agreements (SLAs):** Implemented a P1 (Priority 1) resolution SLA clock set to 4 hours with automated email warning triggers at 50% and 75% elapsed time.
*   **Service Catalog Item:** Created a custom "IT Hardware Request" catalog item complete with workflow approval routing to department managers.

## System Architecture Lifecycle
1. **Incident Ingestion:** User submits a ticket via Service Portal or Email.
2. **Classification:** Ingestion triggers Client Scripts to automatically set Urgency and Impact.
3. **Routing:** Business Rules evaluate properties and assign the ticket to the correct group.
4. **SLA Monitoring:** The SLA engine tracks progress and alerts managers if a breach is imminent.
5. **Resolution:** Fulfiller resolves the incident, triggering an automated closure notification to the end user.
