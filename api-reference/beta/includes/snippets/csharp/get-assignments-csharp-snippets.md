---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d0b07faa09a4ad952dac15b03023b4ac4feff510
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35720291"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var assignments = await graphClient.PrivilegedRoles["{id}"].Assignments
    .Request()
    .GetAsync();

```