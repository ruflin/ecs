## Logging use case

ECS fields used in logging use cases.

### <a name="logging"></a> Logging fields


| Field  | Description  | Level  | Type  | Example  |
|---|---|---|---|---|
| <a name="id"></a>*id* | *Unique id of the log entry.<br/>* | (use case) | keyword | `8a4f500d` |
| <a name="timestamp"></a>*timestamp* | *Timestamp of the log line.<br/>* | (use case) | date | `2016-05-23T08:05:34.853Z` |
| <a name="message"></a>*message* | *The log message.<br/>This can contain the full log line or based on the processing only the extracted message part. This is expected to be human readable.<br/>* | (use case) | text | `Hello World` |
| <a name="hostname"></a>*hostname* | *Hostname extracted from the log line.<br/>* | (use case) | keyword | `www.example.com` |
| <a name="ip"></a>*ip* | *IP Address extracted from the log line. Can be IPv4 or IPv6.<br/>* | (use case) | ip | `192.168.1.12` |
| <a name="level"></a>*level* | *Log level field. Is expected to be `WARN`, `ERR`, `INFO` etc.<br/>* | (use case) | keyword | `ERR` |
| <a name="line"></a>*line* | *Line number the log event was collected from.<br/>* | (use case) | long | `18` |
| <a name="offset"></a>*offset* | *Offset of the log event.<br/>* | (use case) | long | `12` |
| <a name="source.&ast;"></a>*source.&ast;* | *Describes from where the log entries come from.* |  |  |  |
| <a name="path"></a>*path* | *File path of the file the data is harvested from.<br/>* | (use case) | keyword | `/var/log/test.log` |



