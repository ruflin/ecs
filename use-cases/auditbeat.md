## Auditbeat use case

ECS usage in Auditbeat.

### <a name="auditbeat"></a> Auditbeat fields


| Field  | Description  | Level  | Type  | Example  |
|---|---|---|---|---|
| <a name="module"></a>*module* | *Auditbeat module name.<br/>* | (use case) |  |  |
| <a name="file.&ast;"></a>*file.&ast;* | *File attributes.* |  |  |  |
| <a name="path"></a>*path* | *The path to the file.* | (use case) | keyword |  |
| <a name="target_path"></a>*target_path* | *The target path for symlinks.* | (use case) | keyword |  |
| <a name="type"></a>*type* | *The file type (file, dir, or symlink).* | (use case) | keyword |  |
| <a name="device"></a>*device* | *The device.* | (use case) | keyword |  |
| <a name="inode"></a>*inode* | *The inode representing the file in the filesystem.* | (use case) | keyword |  |
| <a name="uid"></a>*uid* | *The user ID (UID) or security identifier (SID) of the file owner.<br/>* | (use case) | keyword |  |
| <a name="owner"></a>*owner* | *The file owner's username.* | (use case) | keyword |  |
| <a name="gid"></a>*gid* | *The primary group ID (GID) of the file.* | (use case) | keyword |  |
| <a name="group"></a>*group* | *The primary group name of the file.* | (use case) | keyword |  |
| <a name="mode"></a>*mode* | *The mode of the file in octal representation.* | (use case) | keyword | `416` |
| <a name="size"></a>*size* | *The file size in bytes (field is only added when `type` is `file`).* | (use case) | long |  |
| <a name="mtime"></a>*mtime* | *The last modified time of the file (time when content was modified).* | (use case) | date |  |
| <a name="ctime"></a>*ctime* | *The last change time of the file (time when metadata was changed).* | (use case) | date |  |
| <a name="hash.&ast;"></a>*hash.&ast;* | *Hash fields used in Auditbeat.<br/>The hash field contains cryptographic hashes of data associated with the event (such as a file). The keys are names of cryptographic algorithms. The values are encoded as hexidecimal (lower-case).<br/>All fields in user can have one or multiple entries.* |  |  |  |
| <a name="blake2b_256"></a>*blake2b_256* | *BLAKE2b-256 hash of the file.* | (use case) | keyword |  |
| <a name="blake2b_384"></a>*blake2b_384* | *BLAKE2b-384 hash of the file.* | (use case) | keyword |  |
| <a name="blake2b_512"></a>*blake2b_512* | *BLAKE2b-512 hash of the file.* | (use case) | keyword |  |
| <a name="md5"></a>*md5* | *MD5 hash.<br/>* | (use case) | keyword |  |
| <a name="sha1"></a>*sha1* | *SHA-1 hash.<br/>* | (use case) | keyword |  |
| <a name="sha224"></a>*sha224* | *SHA-224 hash (SHA-2 family).<br/>* | (use case) | keyword |  |
| <a name="sha256"></a>*sha256* | *SHA-256 hash (SHA-2 family).<br/>* | (use case) | keyword |  |
| <a name="sha384"></a>*sha384* | *SHA-384 hash (SHA-2 family).<br/>* | (use case) | keyword |  |
| <a name="sha512"></a>*sha512* | *SHA-512 hash (SHA-2 family).<br/>* | (use case) | keyword |  |
| <a name="sha512_224"></a>*sha512_224* | *SHA-512/224 hash (SHA-2 family).<br/>* | (use case) | keyword |  |
| <a name="sha512_256"></a>*sha512_256* | *SHA-512/256 hash (SHA-2 family).<br/>* | (use case) | keyword |  |
| <a name="sha3_224"></a>*sha3_224* | *SHA3-224 hash (SHA-3 family).<br/>* | (use case) | keyword |  |
| <a name="sha3_256"></a>*sha3_256* | *SHA3-256 hash (SHA-3 family).<br/>* | (use case) | keyword |  |
| <a name="sha3_384"></a>*sha3_384* | *SHA3-384 hash (SHA-3 family).<br/>* | (use case) | keyword |  |
| <a name="sha3_512"></a>*sha3_512* | *SHA3-512 hash (SHA-3 family).<br/>* | (use case) | keyword |  |
| <a name="xxh64"></a>*xxh64* | *XX64 hash of the file.* | (use case) | keyword |  |



