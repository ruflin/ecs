## Metricbeat use case

ECS fields used Metricbeat.

### <a name="metricbeat"></a> Metricbeat fields


| Field  | Description  | Level  | Type  | Example  |
|---|---|---|---|---|
| <a name="id"></a>*id* | *Unique id to describe the event.<br/>* | (use case) | keyword | `8a4f500d` |
| <a name="timestamp"></a>*timestamp* | *Timestamp when the event was created.<br/>* | (use case) | date | `2016-05-23T08:05:34.853Z` |
| <a name="version"></a>*version* | *Beat version.<br/>* | (use case) | keyword | `6.0.0-rc2` |
| <a name="name"></a>*name* | *Beat name.<br/>* | (use case) | keyword | `filebeat` |
| <a name="id"></a>*id* | *Unique beat identifier.<br/>* | (use case) | keyword | `8a4f500d` |
| <a name="service.&ast;"></a>*service.&ast;* | *The service fields describe the service for / from which the data was collected.<br/>If logs or metrics are collected from Redis, `service.name` would be `redis`. This allows to find and correlate logs for a specicic service or even version with `service.version`.* |  |  |  |
| <a name="id"></a>*id* | *Unique identifier of the running service.<br/>This id should uniquely identify this service. This makes it possible to correlate logs and metrics for one specific service. For example in case of issues with one redis instance, it's possible to filter on the id to see metrics and logs for this single instance.<br/>* | (use case) | keyword | `d37e5ebfe0ae6c4972dbe9f0174a1637bb8247f6` |
| <a name="name"></a>*name* | *Name of the service data is collected from.<br/>The name is normally the same as the module name.<br/>* | (use case) | keyword | `elasticsearch` |
| <a name="version"></a>*version* | *Version of the service the data was collected from.<br/>This allows to look at a data set only for a specific version of a service.<br/>* | (use case) | keyword | `3.2.4` |
| <a name="host"></a>*host* | *Host address that is used to connect to the service.<br/>This normally contains hostname + port.<br/>REVIEW: Should this be service.uri instead, sometimes it's more then just the host? It could also include a path or the protocol.<br/>* | (use case) | keyword | `elasticsearch:9200` |
| <a name="rtt"></a>*rtt* | *Request round trip time.<br/>How long did the request take to fetch metrics from the service.<br/>REVIEW: THIS DOES NOT EXIST YET IN ECS.<br/>* | (use case) | long | `115` |
| <a name="error.&ast;"></a>*error.&ast;* | *Error namespace<br/>Use for errors which can happen during fetching information for a service.* |  |  |  |
| <a name="message"></a>*message* | *Error message returned by the service during fetching metrics.<br/>* | (use case) | text |  |
| <a name="code"></a>*code* | *Error code returned by the service during fetching metrics.<br/>* | (use case) | long |  |
| <a name="hostname"></a>*hostname* | *Hostname of the system metricbeat is running on or user defined name.<br/>* | (use case) | keyword |  |
| <a name="timezone.offset.sec"></a>*timezone.offset.sec* | *Timezone offset of the host in seconds.<br/>* | (use case) | long |  |
| <a name="id"></a>*id* | *Unique host id.<br/>* | (use case) | keyword |  |
| <a name="module"></a>*module* | *Name of the module this data is coming from.<br/>* | (use case) | keyword | `mysql` |
| <a name="dataset"></a>*dataset* | *Name of the dataset.<br/>This contains the information which is currently stored in metricset.name and metricset.module.<br/>* | (use case) | keyword | `stats` |



