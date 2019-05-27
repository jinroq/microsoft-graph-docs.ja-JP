---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d2052b4991983d5ed3a422f224f2935ab495b964
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34481528"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var secureScoreControlProfile = await graphClient.Security.SecureScoreControlProfiles["{id}"]
    .Request()
    .GetAsync();

```