---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: dbdd24d583cf817b3cae81ec281714f8417322d2
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35739102"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryRole = await graphClient.DirectoryRoles["{id}"]
    .Request()
    .GetAsync();

```