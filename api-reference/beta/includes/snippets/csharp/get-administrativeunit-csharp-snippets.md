---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: cc2a3d07f640ec81ed02f5e7279e075730e36bc0
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36408710"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var administrativeUnit = await graphClient.AdministrativeUnits["{id}"]
    .Request()
    .GetAsync();

```