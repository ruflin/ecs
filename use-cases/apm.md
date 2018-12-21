## APM use case

ECS usage for the APM data.

### <a name="apm"></a> APM fields


| Field  | Description  | Level  | Type  | Example  |
|---|---|---|---|---|
| <a name="id"></a>*id* | *Unique id to describe the event.<br/>* | (use case) | keyword | `8a4f500d` |
| <a name="@timestamp"></a>*@timestamp* | *Timestamp when the event was created in the app / service.<br/>* | (use case) | date | `2016-05-23T08:05:34.853Z` |
| <a name="agent.&ast;"></a>*agent.&ast;* | *The agent fields are used to describe which agent did send the information.* |  |  |  |
| <a name="version"></a>*version* | *APM Agent version.<br/>* | (use case) | keyword | `3.14.0` |
| <a name="name"></a>*name* | *APM agent name.<br/>* | (use case) | keyword | `elastic-node` |
| <a name="service.&ast;"></a>*service.&ast;* | *The service fields describe the service inside which the APM agent is running.* |  |  |  |
| <a name="id"></a>*id* | *Unique identifier of the running service.<br/>* | (use case) | keyword | `d37e5ebfe0ae6c4972dbe9f0174a1637bb8247f6` |
| <a name="name"></a>*name* | *Name of the service the agent is running in. This is normally a user defined name.<br/>* | (use case) | keyword | `user-service` |
| <a name="version"></a>*version* | *Version of the service the agent is running in. This depends on if the service is given a version.<br/>* | (use case) | keyword | `3.2.4` |



