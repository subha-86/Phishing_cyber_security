# Sample Phishing Email with Full Header(HTML format):

Return-Path: <security-alert@paypalsecurity.com>
Received: from unknown (HELO mail.paypalsecurity.com) (192.0.2.50)
    by mail.receiverdomain.com with SMTP; Mon, 26 May 2025 08:15:43 +0000
Received-SPF: fail (mail.receiverdomain.com: domain of paypal.com does not designate 192.0.2.50 as permitted sender)
Authentication-Results: mail.receiverdomain.com;
    spf=fail smtp.mailfrom=paypal.com;
    dkim=none;
    dmarc=fail action=reject header.from=paypal.com
From: "PayPal Support" <security-alert@paypalsecurity.com>
To: victim@example.com
Subject: Urgent: Your PayPal Account Has Been Limited
Date: Mon, 26 May 2025 08:14:00 +0000
MIME-Version: 1.0
Content-Type: text/html; charset=UTF-8
Content-Transfer-Encoding: 7bit

<html>
<body>
<p>Dear Customer,</p>

<p>We detected suspicious activity on your PayPal account. To secure your account, please <a href="http://paypa1.com/verify">click here to verify your identity</a> immediately.</p>

<p>If you do not verify within 24 hours, your account will be permanently limited.</p>

<p>Thank you for your prompt attention.</p>

<p>Regards,<br>PayPal Support Team</p>

</body>
</html>

# Check email headers for discrepancies (using online header analyzer):

SPF: fail — The IP 192.0.2.50 is not authorized to send mail for paypal.com.
DKIM: none — No DKIM signature found, which is unusual for legitimate PayPal emails.
DMARC: fail — DMARC policy failed, meaning the email did not pass domain alignment and authentication.

# Identify suspicious links or attachments
Link in email: http://paypa1.com/verify   --    The domain paypa1.com uses the number "1" instead of the letter "l," a common typo-squatting trick to mimic PayPal.

# Look for urgent or threatening language in the email body
Phrases like “please click here to verify your identity immediately” and “your account will be permanently limited” create a sense of urgency and pressure the recipient to act without thinking.
The clickable text says “click here to verify your identity”, but hovering reveals the URL http://paypa1.com/verify — a domain unrelated to PayPal.
