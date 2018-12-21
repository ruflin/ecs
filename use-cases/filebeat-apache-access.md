## Filebeat Apache use case

ECS fields used in Filebeat for the apache module.

### <a name="filebeat-apache-access"></a> Filebeat Apache fields


| Field  | Description  | Level  | Type  | Example  |
|---|---|---|---|---|
| <a name="id"></a>*id* | *Unique id to describe the event.<br/>* | (use case) | keyword | `8a4f500d` |
| <a name="@timestamp"></a>*@timestamp* | *Timestamp of the log line after processing.<br/>* | (use case) | date | `2016-05-23T08:05:34.853Z` |
| <a name="message"></a>*message* | *Log message of the event<br/>* | (use case) | date | `Hello World` |
| <a name="module"></a>*module* | *Currently fileset.module<br/>* | (use case) | keyword | `apache` |
| <a name="dataset"></a>*dataset* | *Currenly fileset.name<br/>* | (use case) | keyword | `access` |
| <a name="ip"></a>*ip* | *Source ip of the request. Currently apache.access.remote_ip<br/>* | (use case) | ip | `192.168.1.1` |
| <a name="name"></a>*name* | *User name in the request. Currently apache.access.user_name<br/>* | (use case) | keyword | `ruflin` |
| <a name="method"></a>*method* | *Http method, currently apache.access.method<br/>* | (use case) | keyword | `GET` |
| <a name="url"></a>*url* | *Http url, currently apache.access.url<br/>* | (use case) | keyword | `http://elastic.co/` |
| <a name="version"></a>*version* | *Http version, currently apache.access.http_version<br/>* | (use case) | keyword | `1.1` |
| <a name="response.code"></a>*response.code* | *Http response code, currently apache.access.response_code<br/>* | (use case) | keyword | `404` |
| <a name="response.body_sent.bytes"></a>*response.body_sent.bytes* | *Http response body bytes sent, currently apache.access.body_sent.bytes<br/>* | (use case) | long | `117` |
| <a name="referer"></a>*referer* | *Http referrer code, currently apache.access.referrer<br/>NOTE: In the RFC its misspell as referer and has become accepted standard<br/>* | (use case) | keyword | `http://elastic.co/` |
| <a name="user_agent.&ast;"></a>*user_agent.&ast;* | *User agent fields as in schema. Currently under apache.access.user_agent.** |  |  |  |
| <a name="original"></a>*original* | *Original user agent. Currently apache.access.agent<br/>* | (use case) | keyword | `http://elastic.co/` |
| <a name="geoip.&ast;"></a>*geoip.&ast;* | *User agent fields as in schema. Currently under apache.access.geoip.*<br/>These are extracted from source.ip<br/>Should they be under source.geoip?* |  |  |  |
| <a name="..."></a>*...* | *All geoip fields.<br/>* | (use case) | keyword |  |



