## Beats use case

ECS fields used in Beats.

### <a name="beats"></a> Beats fields


| Field  | Description  | Level  | Type  | Example  |
|---|---|---|---|---|
| <a name="id"></a>*id* | *Unique id to describe the event.<br/>* | (use case) | keyword | `8a4f500d` |
| <a name="timestamp"></a>*timestamp* | *Timestamp when the event was created.<br/>* | (use case) | date | `2016-05-23T08:05:34.853Z` |
| <a name="agent.&ast;"></a>*agent.&ast;* | *The agent fields are used to describe by which beat the information was collected.* |  |  |  |
| <a name="version"></a>*version* | *Beat version.<br/>* | (use case) | keyword | `6.0.0-rc2` |
| <a name="name"></a>*name* | *Beat name.<br/>* | (use case) | keyword | `filebeat` |
| <a name="id"></a>*id* | *Unique beat identifier.<br/>* | (use case) | keyword | `8a4f500d` |



