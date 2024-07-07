API real time data to Database via ETL pipeline. Utilized yelp Fusion API (https://docs.developer.yelp.com/docs/fusion-intro)

# Config File
<pre>
[KEYS]
CLIENT_KEY=<YOUR CLIENT KEY>
API_KEY=<YOUR API KEY>


[DATABASE]
host=<HOST NAME>
database=<DB NAME>
username=<USER NAME>
password=<PASSWORD>
port=<PORT
</pre>


# Files
<pre>
auth.py - Contains configuration variable for making HTTP Request

businesssearch.py - Contains class to handle results returned from the search request

databasedriver.py - Contains Connection detials to Postgres database and executing queries

queries.py - Contains queries to create schema and tables in postgres and insert statement format

request.py - Contains class to handle making request to the API

driver.py - Entry point for the application, contains parsing command line arguments and control the program flow.
</pre>

# Run Code
<pre>
python driver.py --term food --location Montreal --price 3
</pre>

# Output
![Name](APIPullToDatabase/Resultsapiyelpdb.png)
