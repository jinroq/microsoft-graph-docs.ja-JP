---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: addcd8d45dcfc12503563234334a3b23600ec6e7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358553"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getYammerDeviceUsageUserCounts = await graphClient.Reports
    .GetYammerDeviceUsageUserCounts("D7")
    .Request()
    .GetAsync();

```