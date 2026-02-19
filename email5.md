# Tech Support Email Bot - Hand-Drawn Workflow

## Main Workflow Diagram

```mermaid
graph TD
    INBOX["📧 Teams Channel Message<br/>Message 1<br/>Message 2<br/>Message 3"]
    
    EXTRACT["<b>Title</b><br/>Tag: New Joinee<br/>━━━━━━━━━━━━━━━━━━━━━━<br/>Summary line 1<br/>Summary line 2<br/>━━━━━━━━━━━━━━━━━━━━━━"]
    
    ACCEPT["Accept"]
    REJECT["Reject"]
    REVIEW["Review"]
    ERROR["System Error"]
    
    REASON1["Reason"]
    REASON2["Store Incident in logs"]
    
    DONE["Done"]
    
    PROCESS["Service Catalog"]
    
    INBOX --> EXTRACT
    EXTRACT --> ACCEPT
    EXTRACT --> REJECT
    EXTRACT --> REVIEW
    EXTRACT --> ERROR
    ACCEPT --> PROCESS
    PROCESS --> DONE
    DONE --> REASON2
    REJECT --> REASON1
    REASON1 --> REASON2
    REVIEW --> REASON1
    ERROR --> REASON1
```


## Weekly Dashboard Workflow

```mermaid
graph LR
    DASHBOARD["<b>Weekly Dashboard</b><br/>━━━━━━━━━━━━━━━━━━<br/>Tickets Page<br/>Approve | Req<br/>━━━━━━━━━━━━━━━━━━"]
    
    SYSECO["Sys/Eco"]
    
    STORE["Store Inc"]
    
    DASHBOARD --> SYSECO
    SYSECO --> STORE
```
