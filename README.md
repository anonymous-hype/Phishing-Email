# Phishing Email Analysis Report

## Email Metadata
- **From:** "Amazon Account Security" <no-reply@amaz0n-security.com>  
- **Subject:** "URGENT: Unauthorized Login Attempt Detected"  

## Phishing Indicators Found

### 1. Suspicious Sender Address
- **Claimed Identity:** Amazon  
- **Actual Domain:** `amaz0n-security.com` (uses a zero instead of 'o')  
- **Red Flag:** Not an official Amazon domain (`amazon.com`).  

### 2. Email Headers Analysis
- **SPF Result:** `neutral` (weak authentication).  
- **DKIM:** Passed but for a fake domain.  
- **IP Address:** `192.0.2.123` (TEST-NET range, not Amazon's real servers).  

### 3. Urgent Language
- Keywords: "URGENT," "secure your account immediately."  
- Creates false urgency to bypass logical thinking.  

### 4. Suspicious Link
- **URL:** `http://amaz0n-security-verify.com/account/login`  
- **Red Flags:**  
  - Non-HTTPS link (no encryption).  
  - Fake domain mimicking Amazon.  

### 5. Generic Greeting
- "Dear Customer" instead of your actual name.  

### 6. Technical Red Flags
- Uses `quoted-printable` encoding (common in spam).  
- Hosts logo on HTTP (not HTTPS).  

## Conclusion  
This email exhibits multiple phishing traits: domain spoofing, urgency tactics, and malicious links. Users should **never** click such links and report it to the real organization.  
