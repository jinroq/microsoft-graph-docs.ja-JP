---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4229e474da7edf3e74c5cd0850ba62e987bad000
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36324709"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetOffice365GroupsActivityCounts("D7")
    .Request()
    .GetAsync();

```