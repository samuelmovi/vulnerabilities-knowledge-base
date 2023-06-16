---
name: jQuery UI library with known vulnerabilities
severity: low
cvss-score: 4.8
cvss-vector: CVSS:3.0/AV:N/AC:H/PR:N/UI:N/S:U/C:L/I:L/A:N
cwe-id: CWE-1035
cwe-name: OWASP Top Ten 2017 Category A9 - Using Components with Known Vulnerabilities
compliance:
  owasp10: A5, A6
  pci: '6.2'

---            

The application uses an outdated version of the jQuery UI library, which has known vulnerabilities.

## How to fix

{% tabs jquery-ui-library-with-known-vulnerabilities %}
{% tab jquery-ui-library-with-known-vulnerabilities generic %}
To fix this issue, please update JQuery UI to the latest available version on its official website.

Do not forget to update all the jQuery UI files you have on the server.
{% endtab %}

{% endtabs %}