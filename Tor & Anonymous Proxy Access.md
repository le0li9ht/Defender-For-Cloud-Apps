Query for TOR and Anonymous Proxy IP connections
```
CloudAppEvents
| where TimeGenerated >ago(90d)
| where IPTags has_any ('Tor','Anonymous proxy')
```
