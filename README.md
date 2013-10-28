CloudCmd REST
=============
**/api/v1/**

|Name         |Method   |Body           |Description                    |
|:------------|:--------|:--------------|:------------------------------|
|``fs``       |GET      |               |get file or dir content        |
|             |PUT      |file content   |create/save file               |
|             |DELETE   |               |delete file                    |
|``fs?size``  |GET      |               |get dir size                   |
|``fs?dir``   |GET      |               |get dir content                |
|             |PUT      |               |create dir                     |
|             |DELETE   |               |delete dir                     |
|``fs?files`` |DELETE   |Array of names |delete files                   |
|``mv``       |PUT      |{from, to}     |mv file/dir                    |
|``cp``       |PUT      |{from, to}     |copy file                      |
|``zip``      |PUT      |{from}         |zip file                       |
