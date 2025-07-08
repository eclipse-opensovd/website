# Eclipse OpenSOVD

Modern vehicles are increasingly complex, requiring standardized, interoperable communication protocols for diagnostics and maintenance. The Service-Oriented Vehicle Diagnostics (SOVD) standard, defined in [ISO 17978](https://www.iso.org/standard/85133.html), addresses this need by specifying a service-based architecture for secure and scalable access to diagnostic data and functions. However, the automotive ecosystem lacks open-source implementations that developers, researchers, and OEMs can use to experiment, validate, or integrate SOVD into software-defined vehicles (SDVs).

Eclipse OpenSOVD fills this gap by delivering a freely available, collaboration-driven implementation of ISO 17978, fostering innovation, reducing vendor lock-in, and accelerating industry-wide adoption of standardized diagnostics.

### Scope

Eclipse OpenSOVD provides an open-source implementation of the Service-Oriented Vehicle Diagnostics (SOVD) standard, as defined in [ISO 17978](https://www.iso.org/standard/85133.html).

**In-scope:**

- **Core SOVD Implementation:**

  - Modular, extensible software stack aligned with ISO 17978, including:
    - Server/client implementations for testing, validation, and integration.
    - Legacy compatibility via adapters (e.g., SOVD-to-UDS protocol translation).

- **Security & Compliance:**

  - Authentication/authorization via OAuth 2.0, OpenID Connect, and certificate-based mechanisms.
  - Alignment with ISO 21434 cybersecurity standards for secure data handling.

- **Documentation & Testing:**

  - Comprehensive guides for developers, OEMs, and repair shops.
  - Test suites covering ISO 17978 compliance, edge cases, and interoperability.
  - Example use cases (e.g., OTA updates, predictive maintenance workflows).

### Description

Eclipse OpenSOVD provides an open-source implementation of the Service-Oriented Vehicle Diagnostics (SOVD) standard, as defined in [ISO 17978](https://www.iso.org/standard/85133.html). The project delivers a modular, standards-compliant software stack that enables secure and efficient access to vehicle diagnostics over service-oriented architectures. By offering an open and community-driven implementation, Eclipse OpenSOVD serves as a foundation for developers, OEMs, and tool vendors to build, test, and integrate SOVD-based solutions. The project will hence facilitate adoption and ensure industry coherence with the standard.

Eclipse OpenSOVD complements and integrates the Eclipse S-CORE project by providing an open implementation of the SOVD protocol that can be used for diagnostics and service orchestration within the S-CORE environment. This integration ensures that diagnostic capabilities are natively supported in SDV architectures, enabling developers and OEMs to build more robust, maintainable, and standards-compliant vehicle software stacks.

**Key components include:**

- **SOVD Gateway:** REST/HTTP API endpoints for diagnostics, logging, and software updates.
- **Protocol Adapters:** Bridging modern HPCs (e.g., AUTOSAR Adaptive) and legacy ECUs (e.g., UDS-based systems).
- **Diagnostic Manager:** Service orchestration for fault reset, parameter adjustments, and bulk data transfers.

## Usage

Stay tuned documentation will come soon.

## Contribution

This project welcomes contributions and suggestions. Before contributing, make sure to read the
[contribution guideline](CONTRIBUTING.md).

## Licenses

Apache License, Version 2.0

## Project Scheduling

**Phase 1 (Months 0–12):**

- **Initial Contribution:** Existing codebase integrated into Eclipse infrastructure.
- **Q1–Q2:** Core SOVD API implementation (diagnostic data access, session management).
- **Q3:** Server/client prototypes, test suites, and basic documentation.
- **Q4:** Security hardening (OAuth 2.0/OpenID Connect), legacy adapter modules (SOVD2UDS).

**Phase 2 (Months 13–18):**

- **COVESA alignment (semantic APIs) and Extended Vehicle logging support.**
- **Community-driven pilot deployments with EV OEMs.**

**Phase 3 (Months 19–24):**

- **Edge AI/ML extensions and ISO/DIS 17978-1.2 compliance.**

## Source Code

**Initial Contribution**

**Core Components:**

- **SOVD Gateway:** REST/HTTP API endpoints for diagnostics.
- **Diagnostic Manager:** Session orchestration, fault reset logic.
- **Basic SOVD2UDS adapter:** Protocol translation for legacy ECUs.
