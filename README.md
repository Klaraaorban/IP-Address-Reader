# IP Address Reader🕵️‍♂️🔒

A Python script to parse web server access logs and generate monthly and yearly reports of unique visitors, grouped by anonymized IP prefixes.

This code unfortunatelly can't give the 100% correct number of visitors because of the access log it is given. 

This access log doesn't contain any description about the person 

**-->** this way I can't eliminate if the person has opened the site from multiple IP addresses as well.

Duplicate detection happens only by the basis of time and octets.

## Features✨
- **Regex Log Parsing**: Extracts IP, timestamp, HTTP method, and URL from access logs.
- **Unique Visitor Grouping**: Aggregates IPs by the first three octets (e.g., `192.168.1`) - this is good for duplicate detection.
- **Monthly and Yearly Reports**: Generates `monthly_visitors_report.txt` and `yearly_visitors_report.txt`.
- **Privacy-Conscious**: Tracks visitors without storing full IPs - also duplicate detection.
