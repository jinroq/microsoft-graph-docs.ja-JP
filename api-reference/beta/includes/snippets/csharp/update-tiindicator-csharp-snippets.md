---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2d3094d8f23eb96ce9f00dddbc4302cb7142ea3e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724475"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tiIndicator = new TiIndicator
{
    AdditionalInformation = "additionalInformation-after-update",
    Confidence = 42,
    Description = "description-after-update"
};

await graphClient.Security.TiIndicators["{id}"]
    .Request()
    .Header("Prefer","return=representation")
    .UpdateAsync(tiIndicator);

```