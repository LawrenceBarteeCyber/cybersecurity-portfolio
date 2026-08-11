Phishing Email Investigation

Project Type

Simulated Security Investigation

Status

✅ Completed

Organization

Northstar Financial Services — Simulated Environment

Investigation Overview

An employee reported a suspicious email claiming that their Microsoft 365 account would be suspended unless they verified their account within 30 minutes.

The investigation was conducted to determine whether the message represented a legitimate security notification or a phishing attempt.

⸻

Email Evidence

Subject: URGENT: Your Microsoft 365 account will be suspended

Sender: Microsoft 365 Support <support@m1crosoft-security.com>

Reported URL:

https://m1crosoft-security.example/verify

Employee Action: Link clicked

Credentials Entered: Unknown

⸻

Indicators of Phishing

Several characteristics indicated that the email was suspicious:

1. Lookalike Domain

The sender used:

m1crosoft-security.com

The domain uses a visually similar spelling of “Microsoft” by replacing the letter i with the number 1.

This is consistent with a lookalike or typosquatting domain technique.

2. Urgency and Threats

The message stated that the employee had only 30 minutes to verify the account or risk permanent suspension.

This creates urgency and pressure, which are common social-engineering techniques.

3. Suspicious Verification Link

The email directed the employee to a verification page using a domain that was not associated with Microsoft’s legitimate services.

4. Email Authentication Failures

The security gateway reported:

* SPF: FAIL
* DKIM: FAIL
* DMARC: FAIL

All three authentication checks failed, increasing the likelihood that the message was fraudulent.

5. Recently Registered Domain

The sender domain was reported as recently registered, which further increased suspicion.

⸻

Analyst Assessment

The available evidence indicates that the email was a likely phishing attempt designed to create urgency and potentially obtain the employee’s Microsoft 365 credentials.

The combination of a lookalike domain, suspicious verification URL, urgency, recently registered domain, and failed email authentication checks significantly increased the risk of credential theft.

Because the employee clicked the link, additional investigation would be required to determine whether credentials were entered or whether the account was subsequently compromised.

⸻

Recommended Response

Immediate Actions

1. Report and escalate the phishing message to the security team.
2. Determine whether the employee entered credentials.
3. Secure or reset the affected account if credential exposure is suspected.
4. Review the employee’s authentication activity for suspicious logins.
5. Block the malicious domain and URL where appropriate.

Additional Investigation

6. Search the organization’s mailboxes for the same phishing message.
7. Identify other employees who may have clicked the link.
8. Review affected accounts for suspicious authentication activity.
9. Determine whether any additional malicious activity occurred after the link was accessed.

Prevention

10. Reinforce phishing awareness training.
11. Continue monitoring suspicious domains and email activity.
12. Encourage users to independently verify unexpected account-security messages.

⸻

Incident Classification

Category: Phishing / Social Engineering

Potential Impact: Credential Theft / Account Compromise

Risk Level: High

Confidence: High likelihood of phishing based on available indicators.

⸻

Skills Demonstrated

* Phishing identification
* Email security analysis
* Social-engineering detection
* Domain analysis
* Email authentication concepts
* Incident response
* Security investigation
* Risk assessment
* Security documentation

⸻

Limitations

This project uses simulated email and security-gateway evidence for educational and portfolio purposes.

No real phishing campaign, user account, credentials, or production environment was accessed.

Future Improvements

A future version will reproduce the investigation in a controlled laboratory environment and include screenshots, email headers, URL-analysis evidence, and additional technical artifacts.