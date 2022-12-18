KQL (Kusto Query Language) is a powerful and flexible language that can be used to query and analyze data stored in Azure Monitor logs. It is particularly useful for real-time threat detection because it allows you to quickly and easily identify patterns and anomalies in your data that may indicate a potential threat.

To use KQL for real-time threat detection, you can set up alerts that trigger when certain conditions are met. For example, you might set up an alert to trigger when a high number of failed login attempts are detected within a short period of time, which could indicate a brute-force attack.

Here is an example KQL query that you could use to set up an alert for failed login attempts:

    SecurityEvent
    | where EventID == 4625
    | summarize count() by AccountName, bin(TimeGenerated, 1h)
    | where count_ > 50

This query counts the number of failed login attempts by account name and groups them into 1-hour bins. It then filters the results to only include bins where the count is greater than 50, indicating a high number of failed login attempts in a short period of time.

You can use this query as the basis for an alert by setting the threshold for the number of failed login attempts and the time period you want to consider. For example, you might set the threshold to 50 failed login attempts within an hour, and have the alert trigger if that threshold is exceeded.

To learn more about using KQL for real-time threat detection, I recommend reviewing the documentation provided by Azure Monitor. This will provide more information on the different types of data that are available in Azure Monitor logs, as well as the various operators and functions that you can use in your KQL queries.