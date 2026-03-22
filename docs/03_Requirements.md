# Product Requirements - RoomLight

This document outlines the functional and non-functional requirements for the RoomLight hotel lighting management system.

| ID         | Description                                                                                                     | Type           | Priority |
| :--------- | :-------------------------------------------------------------------------------------------------------------- | :------------- | :------- |
| **REQ-01** | The system shall provide a "Master Switch" (All Off) functionality with a single interaction.                   | Functional     | High     |
| **REQ-02** | Users must be able to create and save lighting profiles (e.g., "Standard", "Suite", "Summer") in the dashboard. | Functional     | High     |
| **REQ-03** | The system must support mass synchronization of configurations to multiple rooms simultaneously.                | Functional     | High     |
| **REQ-04** | The system shall support physical input points at the entrance, bedside, and bathroom.                          | Functional     | Medium   |
| **REQ-05** | The latency between a physical switch press and the light response must be less than 200 ms.                    | Non-functional | High     |
| **REQ-06** | The management interface must be accessible via a standard web browser without additional software.             | Non-functional | Medium   |
| **REQ-07** | The system architecture must support at least 500 individual rooms within a single local network.               | Non-functional | Medium   |
| **REQ-08** | Hotel guests shall not be able to modify the underlying logic or configuration of the switches.                 | Non-functional | High     |
| **REQ-09** | The system shall log hardware failures (e.g., offline controllers or broken bulbs) for maintenance.             | Functional     | Low      |
| **REQ-10** | The management dashboard UI must be customizable to match the hotel brand's visual identity.                    | Non-functional | Low      |
