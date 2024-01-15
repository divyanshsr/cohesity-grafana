# cohesity-grafana
Integration scripts between a cohesity cluster and a grafana dashboard. This dashboard is meant for the visualization of cluster performance and additional reporting capabilities with customizable components.

# DISCLAIMER!

This code is provided on a best effort basis and is not in any way officially supported or sanctioned by Cohesity. The code is intentionally kept simple to retain value as example code. The code in this repository or any affiliated private branches is provided as-is and the author accepts no liability for damages resulting from its use. 

# Instructions: Accessing the API and Postgres credentials
Step 1: Start by accessing the VIP address or Node IP address.

Step 2: Access the Cohesity UI, (https://FQDN/dashboards/summary)

Step 3: Once logged in, access the REST API endpoint, (https://FQDN/irisservices/api/v1/public/postgres)

Step 4: Endpoint documentation: https://developer.cohesity.com/apidocs/71/#/http/api-endpoints/custom-reporting/get-postgres

Step 5: Copy the response and keep the details handy.
