---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d4df16ee11685a1b4d429214ba577f4c26eef537
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35710486"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var alert = await graphClient.Security.Alerts["{id}"]
    .Request()
    .GetAsync();

```