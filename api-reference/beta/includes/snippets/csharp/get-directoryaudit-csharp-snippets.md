---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6b9bc131b594351a1546a32763bf6f2f79463783
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706849"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryAudit = await graphClient.AuditLogs.DirectoryAudits["{id}"]
    .Request()
    .GetAsync();

```