# go-email-verifier
## How this program verifies if an email is legit:
It checks if the email domain has the following records set up.

1) MX -  Mail Exchange:
Checks if the Mail Exchange for the domain has been set up in the DNS.

2) SPF - Sender Policy Framework:
Checks if the domain has set up SPF records with the authorized IPs that are allowed to send mail from this domain.

3) DMARC -  Domain-based Message Authentication Recporting and Conformance:
Checks if the domain has set up DMARC records with the list of action what should be done if the emailing server fails to pass the SPF and DKIM check.

### TODO
Verify DKIM (DomainKey Identified Mail) for the tested domain.

Reference:
1) [Cloudfare - Blog](https://www.cloudflare.com/learning/email-security/dmarc-dkim-spf/)
2) [Youtube - Building this application](https://youtu.be/9E4UEsWpYvM?si=mkYOsaWpnMvVR1Tj)