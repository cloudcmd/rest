CloudCmd REST
=============
**/api/v1/**

|Name         |Method   |Query          |Body               |Description                    |
|:------------|:--------|:--------------|:------------------|:------------------------------|
|`fs`         |`GET`    |               |                   |get file or dir content        |
|             |         |`size`         |                   |get dir or file size           |
|             |         |`time`         |                   |get time of file change        |
|             |         |`hash`         |                   |get file hash                  |
|             |         |`beautify`     |                   |beautify js, html, css         |
|             |         |`minify`       |                   |minify js, html, css           |
|             |`PUT`    |               |file content       |create/write file              |
|             |         | `unzip`       |file content       |unzip and create/write file    |
|             |         | `dir`         |                   |create dir                     |
|             |`PATCH`  |               |diff               |patch file                     |
|             |`DELETE` |               |                   |delete file                    |
|             |         |`files`        |Array of names     |delete files                   |
|`mv`         |`PUT`    |               |{from, to}         |rename file/dir                |
|             |         |               |{from, names, to}  |mv files/dirs                  |
|`cp`         |`PUT`    |               |{from, names, to}  |copy files                     |
|`zip`        |`PUT`    |               |{from}             |pack file                      |
|`unzip`      |`PUT`    |               |{from}             |unpack file                    |
|`config`     |`GET`    |               |                   |get config                     |
|             |`PATCH`  |               |{option:value}     |change config                  |
|`markdown`   |`GET`    |               |                   |parse markdown with path       |
|             |         |`relative`     |                   |parse with relative path       |
|             |`PUT`    |               |raw markdown       |parse raw markdown             |
