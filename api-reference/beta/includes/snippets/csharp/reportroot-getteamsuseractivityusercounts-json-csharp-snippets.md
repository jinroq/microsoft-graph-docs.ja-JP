---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 033c7d57eecd766f213d3a8b1f535ee86068ccf3
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358789"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getTeamsUserActivityUserCounts = await graphClient.Reports
    .GetTeamsUserActivityUserCounts("D7")
    .Request()
    .GetAsync();

```