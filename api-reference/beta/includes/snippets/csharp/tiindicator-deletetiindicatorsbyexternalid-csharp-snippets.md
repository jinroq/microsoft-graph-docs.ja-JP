---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 189b925094f47910764415b4b8f03a55de894ce1
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35716932"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var value = new List<String>()
{
    "externalId-value1",
    "externalId-value2"
};

await graphClient.Security.TiIndicators
    .DeleteTiIndicatorsByExternalId(value)
    .Request()
    .PostAsync();

```