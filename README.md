CloudCmd REST
=============
**/api/v1/**

|Name         |Method   |query          |Body           |Description                    |
|:------------|:--------|:--------------|:--------------|:------------------------------|
|``fs``       |`GET`    |               |               |get file or dir content        |
|             |         |`size`         |               |get dir or file size           |
|             |         |`time`         |               |get time of file change        |
|             |         |`hash`         |               |get file hash                  |
|             |`PUT`    |               |file content   |create/save file               |
|             |         | `dir`         |               |create dir                     |
|             |`DELETE` |               |               |delete file                    |
|             |         | `dir`         |               |delete dir                     |
|             |         |`files`        |Array of names |delete files                   |
|``mv``       |`PUT`    |               |{from, to}     |mv file/dir                    |
|``cp``       |`PUT`    |               |{from, to}     |copy file                      |
|``zip``      |`PUT`    |               |{from}         |zip file                       |
|``config``   |`PUT`    |               |{option:value} |change config                  |
|``markdown`` |`GET`    |               |               |parse markdown with path       |
|             |         |`relative`     |               |parse with relative path       |
|             |`PUT`    |               |markdown       |parse with relative path       |
