---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1ffff0f83acf0370ac8c8b14ada9a112267e1630
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36321781"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSharePointSiteUsageFileCounts("D7")
    .Request()
    .GetAsync();

```