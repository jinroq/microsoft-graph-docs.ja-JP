---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c73859c17bc388ff6774e117b6835d041680607d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358956"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getTeamsDeviceUsageUserDetail = await graphClient.Reports
    .GetTeamsDeviceUsageUserDetail("D7")
    .Request()
    .GetAsync();

```