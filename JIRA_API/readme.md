
# detail jira python API 
http://jira.readthedocs.io/en/latest/examples.html#searching



# have used 
## search_issues

search_issues(jql_str, startAt=0, maxResults=50, validate_query=True, fields=None, expand=None, json_result=None)[source]
Get a ResultList of issue Resources matching a JQL search string.

Parameters:	
jql_str – the JQL search string to use
startAt – index of the first issue to return
maxResults – maximum number of issues to return. Total number of results is available in the total attribute of the returned ResultList. If maxResults evaluates as False, it will try to get all issues in batches.
fields – comma-separated string of issue fields to include in the results
expand – extra information to fetch inside each resource
json_result – JSON response will be returned when this parameter is set to True. Otherwise, ResultList will be returned.

