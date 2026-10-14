Version: NAFATH-V1

Track: Cybersecurity

## Overview

A government single sign-on service allows citizens to access multiple digital services using one account. Developing such a service requires cooperation between software systems, artificial intelligence, mobile applications, networking, cybersecurity, and data protection. OAuth 2.0 supports authorization, while OpenID Connect adds an identity layer for user authentication. AI can help identify unusual login patterns, but its results should be monitored for errors and risks. Mobile applications should manage permissions carefully to protect personal information. DNS over HTTPS helps protect DNS queries during transmission, but it does not provide complete online privacy. Oman's Personal Data Protection Law establishes requirements for handling personal data. The cybersecurity question explored in this research is what makes an authentication method phishing-resistant and which multi-factor authentication methods qualify.


## Software

OAuth 2.0 primarily handles authorization, allowing applications to access protected resources with permission. However, it does not inherently provide user authentication. OpenID Connect (OIDC) adds an identity layer on top of OAuth 2.0, enabling applications to verify a user's identity. OAuth 2.0 mainly uses Access Tokens to grant access to resources, while OpenID Connect uses an ID Token to provide information about the authenticated user.

Resource: Okafor, B. (2021). *OAuth 2.0 and OpenID Connect for Secure Authentication and Token Management in Microservices*. ResearchGate. https://www.researchgate.net/publication/412986363_OAuth_20_and_OpenID_Connect_for_Secure_Authentication_and_Token_Management_in_Microservices

## AI

Artificial intelligence can help identify unusual login patterns that may indicate suspicious activity. However, AI systems may produce false alerts or fail to detect some threats. The NIST AI Risk Management Framework highlights the importance of accuracy, reliability, security, privacy, fairness, and transparency in trustworthy AI systems. Organizations should evaluate and monitor these systems regularly to manage risks, reduce errors, and protect users.

Resource: National Institute of Standards and Technology (NIST). (2023). *Artificial Intelligence Risk Management Framework (AI RMF 1.0).* https://nvlpubs.nist.gov/nistpubs/ai/nist.ai.100-1.pdf

## Mobile

Android uses a permission-based security model to protect user data and system resources. Each application runs under a unique user ID. However, applications may request more permissions than necessary, creating risks to personal information. The study proposes a method combining static and runtime analysis to identify applications with excessive permissions. The authors also explain that this analysis may produce false positive alarms when some application code paths are not tested.

Resource: Geneiatakis, D., Fovino, I. N., Kounelis, I., & Stirparo, P. (2015). *A Permission Verification Approach for Android Mobile Applications*. Computers & Security, 49, 192–205. https://www.sciencedirect.com/science/article/abs/pii/S0167404814001515


## Networking

DNS over HTTPS (DoH) sends DNS queries and responses through HTTPS, helping protect them from being read or modified while traveling across the network. It makes DNS queries harder for third parties to monitor. However, DoH does not hide all network activity or prevent every form of traffic analysis. It mainly protects DNS queries during transmission and does not provide complete online privacy.

Resource: Hoffman, P., & McManus, P. (2018). *DNS Queries over HTTPS (DoH).* RFC 8484. https://www.rfc-editor.org/rfc/rfc8484.html

## Cybersecurity

Phishing resistance is the ability of an authentication protocol to prevent the disclosure of authentication secrets and valid authenticator outputs to an impostor verifier. NIST explains that authentication methods requiring users to manually enter an authenticator output, such as one-time passwords (OTP), are not considered phishing-resistant. An attacker may relay the entered code to the legitimate verifier and successfully authenticate.

Resource: National Institute of Standards and Technology (NIST). *Authenticator and Verifier Requirements*, Section 3.2.5, "Phishing Resistance." https://pages.nist.gov/800-63-4/sp800-63b/authenticators/

## Data

Under Oman's Personal Data Protection Law, organizations must obtain the required consent before processing personal data and inform individuals about the purpose of processing and their rights. They must protect the confidentiality of personal data, establish appropriate procedures for handling it, and maintain records of processing activities. When a personal data breach occurs, the controller must notify the Ministry and the affected individual as required by the law and its Executive Regulations.

Resource: Sultanate of Oman. (2022). *Royal Decree 6/2022 Promulgating the Personal Data Protection Law.* https://prod.mtcit.gov.om/ITAPortal/MediaCenter/Document_detail.aspx?NID=10154


## Misconception in My Track

A common misconception in cybersecurity is that all multi-factor authentication (MFA) methods are phishing-resistant. However, the NIST guidelines explain that authentication methods requiring users to manually enter an authenticator output, such as one-time passwords (OTP), are not considered phishing-resistant. This is because an attacker may relay the entered code to the legitimate verifier and successfully authenticate. Therefore, using multiple authentication factors does not automatically make an authentication method phishing-resistant.

Evidence: NIST SP 800-63B, Section 3.2.5, "Phishing Resistance."

## Open Question

How can government organizations choose authentication methods that provide phishing resistance while remaining easy for citizens to use?
