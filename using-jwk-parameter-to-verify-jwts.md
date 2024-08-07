---
name: Using jwk parameter to verify JWTs
severity: high
cvss-score: 7.5
cvss-vector: CVSS:3.0/AV:N/AC:L/PR:N/UI:N/S:U/C:N/I:H/A:N
cwe-id: CWE-345
cwe-name: Insufficient Verification of Data Authenticity
compliance:
  HIPAA: 164.306(a), 164.312(c)(1)
  ISO 27001: A.8.2, A.8.3, A.8.5, A.8.24
  owasp10: A8
  PCI v4.0: pci4-6.2.4

---            

The server is using the key received in the parameter `jwk` on the JWT header to validate the signature. The jwk is a user controllable parameter which means anyone can change your JWTs contents. If the JWT is used to control access to the application, an attacker could take advantage of this vulnerability to forge a token and impersonate other users or even elevate privileges.

## How to fix

{% tabs using-jwk-parameter-to-verify-jwts %}
{% tab using-jwk-parameter-to-verify-jwts generic %}
To fix this issue, you should force the usage of a predefined public key.
{% endtab %}

{% endtabs %}
