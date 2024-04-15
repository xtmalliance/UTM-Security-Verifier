# Security Verification Test Suite for UTM services

## Goal
This project aims to implement a security verification test suite and framework for systems providing Unmanned Traffic Management (UTM) services.

## Introduction
UTM can be considered as critical national infrastructure and one that is primarily digital. From a regulatory standpoint, different aviation regulators are mandating different security mechanisms given the safety focus of the aviation system. For example, the FAA's [Near-Term Approval Process](https://www.faa.gov/uas/advanced_operations/traffic_management) (NTAP) evaluates third-party services based on safety mitigation, including compliance with ISO standards for information security management systems. The FAA released the conclusive report concerning the [UTM Pilot Program](https://www.faa.gov/sites/faa.gov/files/PL_115-254_Sec376_UAS_Traffic_Management.pdf). Within this report, a segment focusing on message security (Section 4.9) advises securing the connection between the UTM node and the Flight Information Management System utilizing OAuth 2.0 for authorization and TLS for ensuring link security with Public Key Infrastructure (PKI) using certificate authorities [e.g., IATF](https://www.icao.int/airnavigation/IATF/Pages/default.aspx) to manage the use of digital certificates.Their primary recommendation encompasses various measures broadly, including the implementation of digital signatures.

Similarly, the EU [Regulation 2021/664 ](https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=CELEX:32021R0664) on U-Space and the accompanying [AMC/GM](https://www.easa.europa.eu/en/document-library/acceptable-means-of-compliance-and-guidance-materials/amc-and-gm-implementing) mandates security management systems and contingency plans, emphasizing a risk-based approach to security risks identification, assessment, and mitigation.  [AMC/GM1](https://www.easa.europa.eu/en/document-library/acceptable-means-of-compliance-and-guidance-materials/amc-and-gm-implementing) Point 3 of Annex V broadly specifies the exchange of relevant operational data and information between U-space service providers and air traffic service providers in accordance with Transport Layer Security 1.2. However, these frameworks does not specify the detailed processes for threat classification and mitigation.

## Background
In this context, [TII](https://tii.ae), a leading research organization and [OpenUTM](https://openutm.net) a leading UTM implementation, co-led a task force within [GUTMA](https://gutma.org) on Secure and Resilient UTM to explore the implications for UTM service providers around security considerations for UTM services, see report PDF here. As a consequence of the task-force, a need to develop tooling and verification mechanism for security considerations was identified. 
The goal of this project it so provide a comprehensive, updated tools that can be run against UTM services to verify compliance against a specific class of ever evolving cyber-securtiy threats. The toolset is aimed to be run routinely against the UTM system under test to monitor conformance and response to security threats. This initiative aims to bolster cybersecurity concerns of regulators associated with certification by establishing a robust security framework grounded in industry standards. 

## Relationship with the UTM Adapter Project

As the UTM eco-system develops, standards are being developed, the [UTM adapter](https://github.com/Dronecode/utm-adapter) project develops a standard way for a GCS or any other UAV control system to interact with a UTM system.
For the initial implementation phase, the verification suite will qualify the implementation of the GCS and the UTM system under test around the UTM services described in the UTM Adapter. In the long term, we aim to expand the security suite to cover additional UTM services and welcome the community's participation developing a test suite to encompass state-of-the-art cyber security capabilities. 

<p align="center">
  <img src="https://github.com/tiiuae/UTM-Security-Verifier/assets/8924200/19df59e1-bae4-43fd-a023-f9f5c7558d75">
</p>

## Scope
This project is divided into two primary phases. Initially, it involves the implementation verification of UTM adapter [API specifications](https://github.com/Dronecode/utm-adapter/blob/main/ussp-api/utm-adapter.yaml) in a Ground Control Station (GCS) and UTM system under test. This phase ensures that the UTM adapter GCS implementation adheres to the specified requirements and functions as intended defined in the specification and in parallel we will aim to qualify the UTM system under test for compliance with UTM adapter data exchange. 
Subsequently, the project focuses on verifying the security features associated with individual UTM services. This comprehensive approach aims to assess the robustness and effectiveness of cybersecurity measures implemented within the UTM ecosystem.
[cyber_verification](https://github.com/govindsi/UTM-Security-Verification-Suite/assets/8924200/f5f8c9c5-0eb2-43b9-8d47-ca052645f269)

## Outcome

## Deliverables
This project has to main deliverables that can be implemented by any GCS and a UTM provider. 

1. A Test framework for testing the [UTM adapter](https://github.com/Dronecode/utm-adapter) functional specifications to ensure that the compliance against the adapter specification is maintained
2. Security test framework for UTM services:
   * Develop test cases to verify each security feature, ensuring that they meet the specified requirements
   * Document the results of the security verification process, including audit logs.
   
## Timeline

  * Evaluation phase: MAY 2023
  * Phase 1: NOV 2023
  * Phase 2: MAR 2024

## Features
- UTM adapter specification verification
- Verification of the Security Capabilities of UTM Services
 ![security_framework](https://github.com/tiiuae/UTM-Security-Verification-Suite/assets/8924200/70875664-3ac0-4b14-90a8-c09a3f9e08df)


## Documentation


## Contributing
Contributions to the project are welcome! If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request following the contribution guidelines.



