---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 189b925094f47910764415b4b8f03a55de894ce1
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35526495"
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