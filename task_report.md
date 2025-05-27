# Objective:
Identify phishing characteristics in a suspicious email sample.

# Description:
A phishing email is a deceptive message designed to trick the recipient into revealing sensitive information by posing as a legitimate entity.

# Steps:

1. Sample Email Acquisition - 
A phishing email sample was obtained from publicly available online sources for the purpose of analysis.

2. Sender Email Address Examination - 
The sender’s email address was scrutinized for signs of spoofing. While the display name appeared legitimate, the actual email domain contained subtle discrepancies, such as misspellings or variations from the official domain, indicating potential fraudulent intent.

3. Email Header Analysis - 
An online email header analyzer was utilized to inspect the email’s technical authentication details. The email failed key authentication protocols including SPF, DKIM, and DMARC, suggesting the message did not originate from an authorized source.

4. Identification of Suspicious Links and Attachments - 
Hyperlinks within the email were examined by hovering to reveal their true destinations. The URLs directed to domains unrelated to the purported sender and included suspicious elements such as unusual top-level domains or URL shortening services. No attachments were present in this sample; however, attachments generally warrant caution.

5. Language and Tone Assessment - 
The email employed urgent and threatening language, aiming to compel immediate action by the recipient. Phrases indicating imminent account suspension or deadlines are typical social engineering tactics designed to create a sense of urgency.

6. URL Mismatch Verification - 
Displayed link texts did not correspond with the actual URLs, evidencing attempts to deceive the recipient regarding the destination of the links.

7. Spelling and Grammar Review - 
The email contained spelling errors and grammatical inconsistencies uncharacteristic of professional correspondence from legitimate organizations, further undermining its credibility.

8. Summary of Phishing Indicators
* Spoofed or altered sender email address
* Failure of SPF, DKIM, and DMARC email authentication checks
* Suspicious and mismatched URLs directing to untrusted domains
* Use of urgent and threatening language to induce panic
* Presence of spelling and grammatical errors
* Generic greetings lacking personalization





