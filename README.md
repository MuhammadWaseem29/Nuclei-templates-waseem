
### Usage

To use the custom templates, run the following commands:

```bash
nuclei -t /path/to/template.yaml -u https://test.php
```

#### Run Templates by Severity:

- **Low Severity:**
  ```bash
  nuclei -u https://test.php -t /home/waseem/Nuclei-templates-w -severity low
  ```
  This command runs the templates against the target URL and filters the results to show only low-severity vulnerabilities.

- **Medium Severity:**
  ```bash
  nuclei -u https://test.php -t /home/waseem/Nuclei-templates-w -severity medium
  ```
  This command runs the templates against the target URL and filters the results to show only medium-severity vulnerabilities.

- **High Severity:**
  ```bash
  nuclei -u https://test.php -t /home/waseem/Nuclei-templates-w -severity high
  ```
  This command runs the templates against the target URL and filters the results to show only high-severity vulnerabilities.

- **Critical Severity:**
  ```bash
  nuclei -u https://test.php -t /home/waseem/Nuclei-templates-w -severity critical
  ```
  This command runs the templates against the target URL and filters the results to show only critical-severity vulnerabilities.

#### Run Templates with Multiple Severities Combined:

- **Combined Severities (High, Critical, Medium):**
  ```bash
  nuclei -u https://test.php -t /home/waseem/Nuclei-templates-w -severity "high,critical,medium"
  ```
  This command runs the templates against the target URL and filters the results to show vulnerabilities of high, critical, and medium severity.

- **All Severities (Low, Medium, High, Critical):**
  ```bash
  nuclei -u https://test.php -t /home/waseem/Nuclei-templates-w -severity "low,medium,high,critical"
  ```
  This command runs the templates against the target URL and shows vulnerabilities of all severities.

For more advanced usage, refer to the Nuclei [documentation](https://nuclei.projectdiscovery.io/).
```
