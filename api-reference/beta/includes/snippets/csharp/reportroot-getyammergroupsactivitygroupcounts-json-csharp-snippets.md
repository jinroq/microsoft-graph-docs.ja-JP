---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6be81240d2c6fba46152834425664b59d85ce098
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358384"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getYammerGroupsActivityGroupCounts = await graphClient.Reports
    .GetYammerGroupsActivityGroupCounts("D7")
    .Request()
    .GetAsync();

```