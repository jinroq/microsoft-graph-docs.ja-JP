---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 76077cd341a2a2a2a243d2ea134b666ac325c2a7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320231"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetYammerGroupsActivityCounts("D7")
    .Request()
    .GetAsync();

```