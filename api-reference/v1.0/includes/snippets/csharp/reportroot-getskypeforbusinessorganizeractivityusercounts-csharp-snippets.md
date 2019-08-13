---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a61f3ac28d3a21f9d3f603f9629ba90eda0c5359
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320738"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSkypeForBusinessOrganizerActivityUserCounts("D7")
    .Request()
    .GetAsync();

```