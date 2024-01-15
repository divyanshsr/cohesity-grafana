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

# Instructions: Registering the cluster as a Postgres source
Step 1: Navigate to the Connections page, http://localhost:3000/connections/add-new-connection

Step 2: Select the Postgresql data source, http://localhost:3000/connections/datasources/grafana-postgresql-datasource

Step 3: Input the values obtained from Step 5 and fill them out as the below, 

>Host URL: (IP Listed from the output above):(Port listed from the output) (Example: 10.26.1.49:27999)
>
>Database name: postgres
>
>Username: reporting_read
>
>Password:(Password as listed from the output)
>
>TLS/SSL Mode: disable

Step 4: Save & test

# Screenshots

"Screenshot of row 1, CPU and Memory Stats"
> ![img_2](https://github.com/divyanshsr/cohesity-grafana/assets/56066329/0128e284-5ed2-4b03-813a-3236eacf028f)

"Screenshot of row 2, IO Performance"
> ![img_3](https://github.com/divyanshsr/cohesity-grafana/assets/56066329/a8e773f1-037d-4098-b1d0-8053dbf9aab1)

"Screenshot of row 3, View Dashboard"
> ![img_4](https://github.com/divyanshsr/cohesity-grafana/assets/56066329/b0b33091-ec2c-42c9-8e6e-ce39476d9b14)

"Screenshot of the entire dashboard"
> ![img_1](https://github.com/divyanshsr/cohesity-grafana/assets/56066329/8b6c5b85-3bb8-43e5-a28a-b73808f5ddf5)

