# TA-Nessus-Essentials
## About The Project
A simple [Splunk](https://www.splunk.com) Technical Add-On (TA) to perform field extractions & create aliases to support the [Common Information Model (CIM)](https://docs.splunk.com/Documentation/CIM/latest/User/Overview), specifically the [Vulnerablities](https://docs.splunk.com/Documentation/CIM/latest/User/Vulnerabilities) datamodel using CSV-formatted exports from Tenable [Nessus Essentials](https://www.tenable.com/products/nessus/nessus-essentials).

## Using the Addon
Install the TA onto Search Heads and Forwarders - you hopefully know your architecture better than I do, and there are no index-time extractions, only search-time.

Add data to Splunk using the `tenable:nessus:vuln` sourcetype. For basic one-time analysis, the `Add Data` feature in the UI or a `oneshot` from the commandline should suffice. Consider setting up an `inputs.conf` on a Universal Forwarder for regular usage.

## Support
This TA is provided without support. Log an Issue on GitHub or reach out to me on Twitter [@drewchurch](https://www.twitter.com/drewchurch) and ask your question.

## Contributing
PRs are welcome.