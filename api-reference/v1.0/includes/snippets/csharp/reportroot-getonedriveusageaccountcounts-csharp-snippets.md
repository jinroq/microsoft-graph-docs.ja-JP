---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2864b5c7a19dc4a1c08e07f7d3731b3443bc01a2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327617"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetOneDriveUsageAccountCounts("D7")
    .Request()
    .GetAsync();

```