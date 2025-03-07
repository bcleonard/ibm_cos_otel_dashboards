# IBM COS OTEL Dashboards

# What

Version 3.19 of the ClevOS introduced support for Open Telemetry collectors. This feature allows for the deployment of Open Telemetry collectors to all of the IBM COS appliances and supports the collection of metrics and sent the metric collection stack of your choice.

# Where can I run these dashboards?

These dashboards are designed to run in grafana.  While there are many products that support OTEL, these dashboards where developed for a grafana stack.

# Included Dashboards

The following dashboards are included in this repository:

* [Impact Assessment](https://raw.githubusercontent.com/bcleonard/ibm_cos_otel_dashboards/refs/heads/main/ImpactAssessment.json) - The purpose of this dashboard is to provide a high level overview of the health of the IBM COS system.

# Adding the dashboards

To add any of the dashboards to your existing Grafana OTEL stack, you'll need to do the following for each stack:

1. In grafana, go to Home > Dashboards.
1. Select the "New" button in the upper right hand side of the screen and then "Import".
1. Select one of the dashboard links above.  It should take you to the raw text of the dashboard in json format.
1. Copy the raw text to your clipboard
1. Back in grafana, past the contents into the "Import via dashboard JSON model" text box.
1. Click the Load button.
1. Next you can change the name of the Dashboard (if you want to). the location of the Dashboard into a specific folder.
1. Its recommended to leave the uid.
1. Last "Select a Prometheus data source". This should be an existing Prometheus data source that is already receiving OTEL data from your existing IBM COS solution.
1. Select the "Import" button.
1. You should be presented with the imported dashboard.

# How To Get Help

If you have questions, comments or concerns, the only way to get help is through this repository.  We recommend searching through [issues first](https://github.com/bcleonard/ibm_cos_otel_dashboards/issues).   If you don't find what you're looking for, feel free to open a new issue.   Please do **NOT** open a ticket with IBM Support.   They can't and won't help you.

# Notice

This is repository is provided as-is.  Please don't call IBM Support if you have any questions about these dashboards.

# Acknowledgements

This repository would not be possible without the [IBM OTEL Demo Environment](https://github.com/bcleonard/ibm_otel_demo_environment).  You should be able to use dashboards in this repo with the environment that is stood up with that environment.
