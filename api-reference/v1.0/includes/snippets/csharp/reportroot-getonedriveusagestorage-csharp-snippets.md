---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a43692815d82b49543d8af257b1000527d024afa
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36321872"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetOneDriveUsageStorage("D7")
    .Request()
    .GetAsync();

```