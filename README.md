# Security Verification Test Suite for UTM services

## Goal
This project aims to implement a security verification test suite for the Unmanned Traffic Management (UTM) services.

## Background
From a regulatory standpoint, the FAA's Near-Term Approval Process (NTAP) evaluates third-party services based on safety mitigation, including compliance with ISO standards for information security management systems.
Similarly, the EU Regulation 2021/664 mandates security management systems and contingency plans, emphasizing a risk-based approach to security risks identification, assessment, and mitigation. However, these frameworks
lack detailed processes for threat classification and mitigation.

To address these gaps, TII and openskies led GUTMA Task Force on Secure and Resilient UTM has developed a comprehensive threat template with best practices for mitigation strategies. This initiative aims to bolster cybersecurity concerns
associated with certification by establishing a robust security framework grounded in industry standards.
![security_services](https://github.com/tiiuae/UTM-Security-Verification-Suite/assets/8924200/4e18a024-b188-4a28-a142-c85b073123f9)


For the initial implementation phase, the verification suite will qualify  ![UTM adapter](https://github.com/Dronecode/utm-adapter) specification compatible GCS and ![openUTM](https://github.com/openutm) (FlightBlender),
both of which implement critical services like flight planning, network-remote ID, conformance monitoring, and traffic information.

## Scope
This project encompasses two primary phases. Initially, it involves the implementation verification of UTM adapter specifications.
This phase ensures that the UTM adapter adheres to the specified requirements and functions as intended.
Subsequently, the project focuses on verifying the security features associated with individual UTM services.
This comprehensive approach aims to assess the robustness and effectiveness of cybersecurity measures implemented within the UTM ecosystem.
![cyber_verification](https://github.com/govindsi/UTM-Security-Verification-Suite/assets/8924200/f5f8c9c5-0eb2-43b9-8d47-ca052645f269)

## Outcome

## Deliverables

1. Test framework for ![UTM adapter](https://github.com/Dronecode/utm-adapter) functional specifications
2. Secutity test frameowrk for UTM services.
   * Develop test cases to verify each security feature, ensuring that they meet the specified requirements
   * Document the results of the security verification process, including audit logs.
   
## Timeline

  * Evaluation phase: APR 2023
  * Phase 1: SEP 2023
  * Phase 2: MAR 2024

## Features
- UTM adapter specification verification
- Verification of the Security Capabilities of UTM Services
- ![security_frmework](https://github.com/tiiuae/UTM-Security-Verification-Suite/assets/8924200/70875664-3ac0-4b14-90a8-c09a3f9e08df)


## Documentation


## Contributing
Contributions to the project are welcome! If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request following the contribution guidelines.



