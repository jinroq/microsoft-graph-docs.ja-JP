---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 18d1370cd31f7a54d040f5b797774be0d8bce416
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327432"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetEmailActivityUserCounts("D7")
    .Request()
    .GetAsync();

```