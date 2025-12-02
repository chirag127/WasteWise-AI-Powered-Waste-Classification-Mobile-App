# Security Policy

## Reporting a Vulnerability

We take security seriously. If you believe you have found a security vulnerability in **EcoSnap-AI-Waste-Classification-Mobile-App**, please report it responsibly.

We encourage you to report any security vulnerabilities found in this project. Please follow these steps:

1.  **Discover:** Identify the security vulnerability in the codebase.
2.  **Report:** Submit a detailed report through the GitHub Security Advisory system or by opening a private security vulnerability report.
    *   **GitHub Security Advisory:** Navigate to the "Security" tab of our repository ([https://github.com/chirag127/EcoSnap-AI-Waste-Classification-Mobile-App/security/advisories](https://github.com/chirag127/EcoSnap-AI-Waste-Classification-Mobile-App/security/advisories)) and click on "New advisory".
    *   **Private Security Report:** You can also use the "Report a vulnerability" button on the same page for a more direct and private channel.
3.  **Details:** In your report, please include:
    *   A clear and concise description of the vulnerability.
    *   The affected version(s) of the project.
    *   Steps to reproduce the vulnerability.
    *   Any potential impact or severity assessment.
    *   (Optional) Proposed mitigation steps.

## Supported Versions

At this time, only the latest stable version of **EcoSnap-AI-Waste-Classification-Mobile-App** is actively being reviewed for security issues. Older versions are not guaranteed to be supported.

## Responsible Disclosure Timeline

We aim to acknowledge all security reports within **48 hours**. We will then work with security researchers to understand the vulnerability and develop a fix. We commit to resolving vulnerabilities as quickly as possible and will provide regular updates on the progress.

*   **Acknowledgement:** Within 48 hours of receiving a report.
*   **Triage & Investigation:** Within 7 days.
*   **Fix Development:** Dependent on the severity and complexity of the vulnerability.
*   **Disclosure:** Once a fix is available and deployed, we will coordinate the public disclosure of the vulnerability, typically after a patch is released.

## Security Best Practices

For developers contributing to **EcoSnap-AI-Waste-Classification-Mobile-App**, please adhere to the following security best practices:

*   **Dependency Management:** Keep all dependencies (React Native, Expo, Node.js, etc.) up-to-date with the latest security patches. Use tools like `npm audit` or `yarn audit` regularly.
*   **Data Handling:** Be mindful of sensitive data. Avoid storing personally identifiable information (PII) unnecessarily. Encrypt sensitive data both in transit and at rest where applicable.
*   **Input Validation:** Sanitize and validate all user inputs to prevent injection attacks (e.g., XSS, SQL injection if applicable to any backend services).
*   **API Security:** Secure all API endpoints. Use authentication and authorization mechanisms appropriately. For any AI model interactions, ensure proper sanitization of prompts and outputs.
*   **Code Reviews:** Participate actively in code reviews, specifically looking for potential security flaws.

Thank you for helping to keep **EcoSnap-AI-Waste-Classification-Mobile-App** secure!
