# Artemis Financial: Secure Application Refactoring

This repository contains the refactored code and security assessment for the Artemis Financial application. The project focused on modernizing the application's security posture by implementing cryptographic integrity controls and transitioning communication protocols to secure standards.

### Client and Requirements

Artemis Financial required a comprehensive security overhaul of their legacy application architecture. The primary objective was to mitigate significant security risks inherent in the existing codebase, specifically addressing the lack of encrypted transit and data integrity verification. The company needed to move away from insecure HTTP protocols and implement standard cryptographic methods to protect sensitive financial data.

### Secure Coding and Value

During the vulnerability assessment, I effectively identified and isolated architectural weaknesses by mapping them against a formal process flow. I performed this by prioritizing an architectural review before proceeding to remediation. Coding securely is vital because it protects the organization’s most valuable asset: trust. Software security adds significant value by preventing the high costs associated with data breaches, regulatory fines, and reputational damage. By embedding security into the development lifecycle, we transition from reactive patching to a proactive, resilient architecture.

### Vulnerability Assessment: Challenges and Methodology

The most challenging part of the assessment was navigating the dependency management and ensuring that security headers were correctly mapped without disrupting application functionality. However, utilizing the Vulnerability Assessment Process Flow diagram was incredibly helpful; it provided a structured, logical roadmap that ensured no critical domain (such as Input Validation or Encapsulation) was overlooked.

### Strengthening Security Layers

I increased the application's security through a Defense-in-Depth approach:

* Transit Security: Refactored the application to utilize HTTPS/TLS, ensuring encrypted communication between the client and server.

* Data Integrity: Implemented SHA-256 cryptographic hashing to ensure data remains untampered.
  
In the future, I would leverage Threat Modeling and the OWASP Top 10 to systematically assess risks and select the most effective mitigation techniques based on specific threat vectors.

### Validation and Verification
To ensure the refactored application was both functional and secure, I performed a three-tiered validation:

* Logical Verification: Manually tested endpoints to ensure core business functions remained intact.

* Static Analysis: Ran dependency-check tools to identify any insecure libraries or components introduced during the update.

* Build Validation: Confirmed that the application compiled cleanly in a clean environment, ensuring the stability of the new security implementations.

### Tools and Future Practices
This assignment introduced me to critical industry-standard tools that I plan to use in future projects, including Java Keytool for certificate management, Maven for build automation, and OWASP Dependency-Check for automated vulnerability scanning. These tools, paired with the practice of performing manual code reviews against a defined architectural process, are essential for any secure development lifecycle.

### Professional Portfolio
For future employers, I would highlight this project as a demonstration of my ability to perform Secure Software Development. Specifically, I can provide:

* Technical Artifacts: The refactored Java source code demonstrating cryptographic implementation.

* Analytical Reporting: The security assessment report, which showcases my ability to bridge the gap between architectural theory and practical code remediation.

* Compliance Verification: The dependency reports, which prove my ability to use automated tools to ensure production-ready code quality.
