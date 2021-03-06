---
title: ftp put
description: "Windows Commands topic for FTP - put"

ms.prod: windows-server


ms.technology: manage-windows-commands

ms.topic: article
ms.assetid: 95cc1e3f-523d-4374-98b8-16e6c276b2ca vhorne
author: coreyp-at-msft
ms.author: coreyp
manager: dongill
ms.date: 03/30/2020
---
# ftp: put

> Applies to: Windows Server (Semi-Annual Channel), Windows Server 2019, Windows Server 2016, Windows Server 2012 R2, Windows Server 2012

Copies a local file to the remote computer using the current file transfer type.
## Syntax
```
put <LocalFile> [<remoteFile>]
```
#### Parameters

|    Parameter     |                    Description                    |
|------------------|---------------------------------------------------|
|   `<LocalFile>`  |         Specifies the local file to copy.         |
| `[<remoteFile>]` | Specifies the name to use on the remote computer. |

## Remarks
- The **put** command is identical to the **send** command.
- if *remoteFile* is not specified, the file is given the *LocalFile* name.
  ## Examples
  copy the local file **test.txt** and name it **test1.txt** on the remote computer.
  ```
  put test.txt test1.txt
  ```
  copy the local file **program.exe** to the remote computer.
  ```
  put program.exe
  ```
  ## Additional References
- [ftp: ascii](ftp-ascii.md)
- [ftp: binary](ftp-binary.md)
- - [Command-Line Syntax Key](command-line-syntax-key.md)
