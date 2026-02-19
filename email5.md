# Tech Support Email Bot - Hand-Drawn Workflow

## Main Workflow Diagram

```mermaid
graph LR
    INBOX["📧 Teams Channel Message<br/>Message 1<br/>Message 2<br/>Message 3"]
    
    EXTRACT["<b>Title</b><br/>Tag: New Joinee<br/>━━━━━━━━━━━━━━━━━━━━━━<br/>Summary line 1<br/>Summary line 2<br/>━━━━━━━━━━━━━━━━━━━━━━<br/>Accept | Reject | Review | System Error"]
    
    PROCESS["Service Catalog"]
    
    INBOX --> EXTRACT
    EXTRACT --> PROCESS
```
