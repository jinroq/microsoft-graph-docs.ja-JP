---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 97ec46bb649c0cb899245cd336dbb8e08e374bfc
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35732241"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var destinationId = "destinationId-value";

await graphClient.Me.Messages["{id}"]
    .Copy(destinationId)
    .Request()
    .PostAsync();

```