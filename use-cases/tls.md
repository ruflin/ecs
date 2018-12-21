## TLS use case

You can store TLS-related metadata under `tls.`, when appropriate.


### <a name="tls"></a> TLS fields


| Field  | Description  | Level  | Type  | Example  |
|---|---|---|---|---|
| <a name="ip"></a>*ip* | ** | (use case) |  | `10.1.1.10` |
| <a name="ip"></a>*ip* | ** | (use case) |  | `5.5.5.5` |
| <a name="port"></a>*port* | ** | (use case) |  | `443` |
| <a name="version"></a>*version* | *TLS version.<br/>* | (use case) | keyword | `TLSv1.2` |
| <a name="certificates"></a>*certificates* | *An array of certificates.<br/>* | (use case) | keyword |  |
| <a name="servername"></a>*servername* | *Server name requested by the client.<br/>* | (use case) | keyword | `localhost` |
| <a name="ciphersuite"></a>*ciphersuite* | *Name of the cipher used for the communication.<br/>* | (use case) | keyword | `ECDHE-ECDSA-AES-128-CBC-SHA` |



