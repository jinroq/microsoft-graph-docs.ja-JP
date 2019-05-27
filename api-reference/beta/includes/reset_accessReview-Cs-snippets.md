---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b7877ea77f412edbea4ec16e8bf631caa167455a
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34482144"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.AccessReviews["2975E9B5-44CE-4E71-93D3-30F03B5AA992"]
    .ResetDecisions()
    .Request()
    .PostAsync();

```