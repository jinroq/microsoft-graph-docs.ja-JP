---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e0984a84a80c562a3635df91130665d05c7b9566
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35733426"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var alert = await graphClient.Security.Alerts["{alert_id}"]
    .Request()
    .GetAsync();

```