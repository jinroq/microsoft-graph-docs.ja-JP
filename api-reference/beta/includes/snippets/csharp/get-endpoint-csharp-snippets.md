---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e95994522b0548f957101f3ff5be2408cb42847f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35486838"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var endpoint = await graphClient.Groups["{id}"].Endpoints["{id}"]
    .Request()
    .GetAsync();

```