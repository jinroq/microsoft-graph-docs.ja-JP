---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5491411cb04fee8c9c4f87c88929a0f49718b19d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358804"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getTeamsUserActivityCounts = await graphClient.Reports
    .GetTeamsUserActivityCounts("D7")
    .Request()
    .GetAsync();

```