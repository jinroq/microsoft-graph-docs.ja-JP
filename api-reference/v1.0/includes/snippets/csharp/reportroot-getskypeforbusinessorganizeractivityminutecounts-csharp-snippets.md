---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c675f91f192c282dc237387031094c1d3bb6395c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349217"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSkypeForBusinessOrganizerActivityMinuteCounts("D7")
    .Request()
    .GetAsync();

```