---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7c43be70b95b2beaa466ecb7e8664380b16dead5
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35526790"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryAudits = await graphClient.AuditLogs.DirectoryAudits
    .Request()
    .GetAsync();

```