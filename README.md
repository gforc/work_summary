## work_summary

#connect jira to collect PR information 

```
from jira import JIRA
import re

>connnect jira server with your username and passowrd
jira = JIRA('https://JiraServerIpAdress',basic_auth=('admin', 'admin'))
> select what you needed issues by jql_srt
issues = jira.search_issues(jql_str='assignee=currentUser()')

print(issues)
for key in issues :
> show the specified detail of the issue
    print(key.fields.summary)
    
```
