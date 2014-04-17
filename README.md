CloudCmd REST
=============
**/api/v1/**

|Name         |Method   |query          |Body           |Description                    |
|:------------|:--------|:--------------|:------------------|:------------------------------|
|``fs``       |`GET`    |               |                   |get file or dir content        |
|             |         |`size`         |                   |get dir or file size           |
|             |         |`time`         |                   |get time of file change        |
|             |         |`hash`         |                   |get file hash                  |
|             |`PUT`    |               |file content       |create/write file              |
|             |         | `unzip`       |file content       |unzip and create/write file    |
|             |         | `dir`         |                   |create dir                     |
|             |`DELETE` |               |                   |delete file                    |
|             |         | `dir`         |                   |delete dir                     |
|             |         |`files`        |Array of names     |delete files                   |
|``mv``       |`PUT`    |               |{from, to}         |rename file/dir                |
|``mv``       |`PUT`    |               |{from, names, to}  |mv files/dirs                  |
|``cp``       |`PUT`    |               |{from, names, to}  |copy files                     |
|``zip``      |`PUT`    |               |{from}             |zip file                       |
|``config``   |`PUT`    |               |{option:value}     |change config                  |
|``markdown`` |`GET`    |               |                   |parse markdown with path       |
|             |         |`relative`     |                   |parse with relative path       |
|             |`PUT`    |               |markdown           |parse with relative path       |
