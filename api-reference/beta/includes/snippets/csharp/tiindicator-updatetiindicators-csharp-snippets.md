---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d28ed4a9b659ee6675de1490dfd0eeca9cc02ebc
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35716905"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var value = new List<TiIndicator>()
{
    new TiIndicator
    {
        Id = "c6fb948b-89c5-3bba-a2cd-a9d9a1e430e4",
        AdditionalInformation = "mytest"
    },
    new TiIndicator
    {
        Id = "e58c072b-c9bb-a5c4-34ce-eb69af44fb1e",
        AdditionalInformation = "test again"
    }
};

await graphClient.Security.TiIndicators
    .UpdateTiIndicators(value)
    .Request()
    .PostAsync();

```