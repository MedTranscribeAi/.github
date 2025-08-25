---
layout: default
title: Bug Bounty Program
nav_order: 11
---

**bug-bounty.md**

# MedTranscribe AI Bug Bounty Program

Welcome to the MedTranscribe AI Bug Bounty Program. At MedTranscribe AI, we take the security of our platform seriously and appreciate the efforts of ethical hackers and researchers in helping us protect our users. This bug bounty program outlines our scope, rules of engagement, disclosure guidelines, and rewards for vulnerabilities reported in good faith. **We also provide a Safe Harbor clause** – as long as you follow this policy and act in good faith, we will consider your research authorized and will not pursue legal action (details in the Safe Harbor section below).

## In-Scope Assets

The following targets are in scope for this program. Testing these systems is authorized and eligible for rewards:

-   **Web Application:** The MedTranscribe AI web app (including the main website and any subdomains under medtranscribe.ai).
-   **API Endpoints:** Any official MedTranscribe AI API endpoints (e.g., `api.medtranscribe.ai`).
-   **Mobile Applications:** The MedTranscribe AI mobile apps for iOS and Android (latest published versions).
-   **Other Assets:** Any other assets explicitly listed on our official bug bounty page or documentation as in-scope.

If an asset is not listed above, it should be considered out-of-scope by default (unless you have written permission from us to test it).

## Out-of-Scope Exclusions

For the safety of our users and systems, **do NOT test or report on the following, as they are out-of-scope**:

-   **Third-Party Services:** Vulnerabilities in third-party platforms, libraries, or services that MedTranscribe AI uses but does not control (please report those to the respective vendors).
-   **Denial of Service:** Any attacks that attempt to overwhelm or disrupt our services (DoS/DDoS, brute-force flooding, or mass automation) are prohibited.
-   **Social Engineering & Physical Attacks:** Any social engineering (phishing, vishing, etc.) against our employees or users, or physical attempts to access facilities/data centers, are not allowed.
-   **Security Best Practices Warnings:** Issues that do not pose a concrete security vulnerability (e.g., missing security headers with no exploitable impact, disallowed HTTP methods, or use of older protocols without an actual vulnerability).
-   **Content & UX Bugs:** UI/UX issues, spelling mistakes, or general software bugs that do not have a security impact.
-   **Self-XSS and Safe-Click Issues:** Vulnerabilities that require a victim to intentionally perform unsafe actions (e.g. paste malicious code into their own browser console) are generally not eligible.
-   **Known Issues / Duplicates:** Any vulnerability already known to us or already reported by another researcher (only the first report of an issue is eligible for bounty).

_If you are unsure whether a certain test or asset is allowed, please contact us for clarification before proceeding (see Reporting Process below)._ Testing anything out-of-scope or violating these exclusions may disqualify your submission from rewards and protection.

## Rules of Engagement (Ethical Guidelines)

To ensure a productive collaboration, we ask all participants to **follow these guidelines** when testing and reporting:

-   **Respect Privacy & Data:** Do not access, copy, modify, or delete user data or sensitive information beyond what is necessary to demonstrate the vulnerability. If a vulnerability exposes personal data, **stop testing and report it immediately**. **No data exfiltration** beyond a proof of concept is permitted.
-   **Minimal Disruption:** Perform testing in a manner that does not disrupt our service or degrade the user experience. Avoid techniques that could automatically spam, brute-force, or overload systems. If you discover a critical issue (e.g. system compromise), report it right away and cease further exploitation.
-   **Good Faith Actions:** Test only against in-scope assets and within the bounds of this policy. Do not use findings to compromise other systems or pivot to unrelated networks.
-   **No Social Engineering or Physical Attacks:** As noted, do not attempt to phish, pretext, or socially engineer our staff or users. Likewise, physical intrusion or tampering with infrastructure is strictly off-limits.
-   **Responsible Disclosure:** You **must privately report** all vulnerabilities to us first. **Do not discuss or publicize** any vulnerabilities (including on forums, social media, etc.) before we have mitigated the issue and given you explicit permission. Coordinated disclosure is important for user safety.
-   **No Ransom or Extortion:** Do not attempt to extort money or services by threatening to reveal vulnerabilities. We gladly reward valid reports, so any form of extortion will result in disqualification and possible ban from the program.
-   **Follow Program Terms:** Adhere to all terms of this policy and any other relevant agreements. If there is a conflict between this policy and other terms (including our general Terms of Service), **this policy will prevail for the purpose of security research.** Always comply with applicable laws during your testing.
-   **One Issue per Report:** Submit one vulnerability per report, with clear delineation. If multiple issues are related, you may mention them, but please do not bundle unrelated findings in one submission.
-   **Duplicates & Prior Findings:** As noted, only the first report of a given issue will be considered for a reward. If you discover a vulnerability, report it promptly – duplicate reports might be closed as informative without reward.

By following these rules, you ensure a collaborative, safe testing environment for both the researchers and our team. We reserve the right to disqualify reports that violate these rules or that come from testing beyond what is permitted.

## Rewards

We offer monetary rewards (bug bounties) for **valid, unique security vulnerabilities** that have a real impact on the security or privacy of our users. The bounty amount is determined by the severity of the vulnerability, based on a CVSS-style severity assessment (Critical/High/Medium/Low), as well as other factors like impact, ease of exploitation, and report quality. Below is the **general reward range** for each severity level (all amounts in USD):

| Severity (CVSS v3)      | **Typical Bounty** |
| ----------------------- | ------------------ |
| **Critical** (9.0 – 10) | up to $1,000       |
| **High** (7.0 – 8.9)    | up to $500         |
| **Medium** (4.0 – 6.9)  | up to $200         |
| **Low** (0 – 3.9)       | up to $50          |

> **Note:** These ranges serve as guidelines. The exact reward for a specific report will be at our discretion and may vary based on the specific impact and creativity of the vulnerability. Exceptional reports (especially for novel or severe issues) may receive higher payouts. Conversely, low-quality reports or issues with minimal security impact may receive lower rewards or possibly no reward if deemed not significant enough. We will notify you of the bounty amount upon resolution of the issue.

Only reports that meet the criteria and follow this policy will be eligible for rewards. In particular, vulnerabilities must be previously unknown to us and not publicly disclosed. We do not reward reports for out-of-scope issues or those that we determine to be false positives. **If two researchers report the same issue, only the first report (based on submission time) is eligible for a bounty.**

## Reporting Process

We encourage you to submit your findings to us through our **GitHub-based reporting channel** or via email. Please use the following process to ensure an effective disclosure:

1. **Prepare Your Report:** Gather all relevant details about the vulnerability. This should include a clear description of the issue, the affected product or page, step-by-step instructions to reproduce it, screenshots or proof-of-concept code if applicable, and an explanation of the potential impact. The more detail you provide, the easier it is for us to triage.
2. **Submit via GitHub or Email:** We prefer that you report the issue by opening a new **GitHub Issue** in this repository using the **Security Vulnerability Report** template (which will guide you to provide all necessary information). This will automatically label the issue as security-related. If you are uncomfortable with a public issue or believe the report is very sensitive, you may alternatively send the report via email to **security@medtranscribe.ai**. (If emailing, please include the same details outlined in the issue template.)
3. **Acknowledgment:** Once you submit a report, our security team will review it. We aim to acknowledge your report within **3 business days**, confirming that we’ve received it and are investigating.
4. **Assessment & Triage:** Our team will validate the issue, determine its severity, and verify that it is in scope. We might reach out to you via the GitHub issue or email for further clarification or to request additional information during this process. Please be responsive to questions.
5. **Resolution:** We will work on fixing the confirmed vulnerability. The time to fix will depend on the complexity and severity. For critical issues, we strive to implement fixes as soon as possible (and in any case, within a reasonable timeframe). We ask for your patience during this period. **Please do not disclose the vulnerability publicly while we are working on a fix.**
6. **Bounty Award & Disclosure:** After the vulnerability has been resolved (or a fix has been deployed), we will coordinate with you to handle the bounty reward. We will notify you of the reward amount (per the guidelines above) and arrange payment. Typically, rewards are paid via electronic means such as PayPal or bank transfer (we will work with you to find a suitable method). At this stage, with the issue fixed, we will also discuss public disclosure. If you would like to publish a write-up or if we include the issue in our release notes, we are happy to credit your contribution publicly (using your name or handle as you prefer). Responsible disclosure means you agree to wait for our confirmation before making any details public.

Throughout this process, we are committed to keeping you informed of our progress and appreciative of your effort. We may provide updates in the GitHub issue or via email at key stages (triage result, fix ETA, etc.). If at any point you need to contact us for an update, feel free to reach out on the issue or via the security email.

## Safe Harbor (Legal Protections)

Our bug bounty program is designed to protect responsible security researchers. **As long as you abide by this policy and submit vulnerabilities in good faith, we promise the following Safe Harbor terms:**

-   **No Legal Action:** MedTranscribe AI will not initiate or support any law enforcement or civil action against you for your security research, **provided you adhere to this policy**. We consider your good-faith research activities to be **authorized** and lawful. Specifically, we consider such activities to be authorized conduct under anti-hacking laws like the Computer Fraud and Abuse Act (CFAA).
-   **Anti-Circumvention Waiver:** We will not bring a DMCA claim or other intellectual property claim against you for circumvention of technological measures, **as long as your testing is within scope** and in line with this policy.
-   **Terms of Service:** Any restrictive language in our website Terms of Service or other policies that would prohibit security testing is waived for actions taken under this bug bounty program. In other words, we won’t consider your testing as a violation of our usage terms, _as long as_ it is done in accordance with this policy.
-   **Good Faith Protection:** We understand that vulnerability research can sometimes cause incidental issues. If you accidentally do something that goes beyond this policy in the process of testing (e.g., trigger an alert or unintentionally access a small amount of data), **let us know immediately**. We will work with you in good faith and not pursue action as long as it was unintentional and no harm was done. We treat all activities following this policy as efforts to improve our security, and **we welcome them**.
-   **Third-Party Actions:** This Safe Harbor applies to legal action under MedTranscribe AI’s control. We cannot bind third parties. If you engage in testing on a third-party asset or service (outside our scope) or a vulnerability affects a third-party, we cannot guarantee that third party won’t pursue legal action. However, **if a third party initiates legal action against you** for activities that were part of our program, MedTranscribe AI will make it known that your actions were conducted pursuant to our bug bounty program and with our authorization. (Always avoid testing third-party systems without permission.)

**Important:** This Safe Harbor is conditional on your compliance with this policy. If your actions are not in good faith or violate the rules of engagement (for example, exploiting data for personal gain, or targeting out-of-scope systems), then this Safe Harbor may be void. You are also expected to comply with all applicable laws. If you have any uncertainty about whether an action might violate this policy, **please ask us first**. We value your research and want to work with you to keep our platform secure.

---

We thank you for helping us keep MedTranscribe AI secure! Your contributions through this bug bounty program make a real difference. If you have any questions about the policy or need clarification on scope, feel free to reach out at security@medtranscribe.ai before you begin. Happy hunting, and we look forward to collaborating with you!
