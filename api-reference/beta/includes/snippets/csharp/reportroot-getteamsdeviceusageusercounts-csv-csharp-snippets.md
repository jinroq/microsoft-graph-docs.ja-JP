---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 30c36e5ff6d0f2f60ce799de0cf6584ea51a2abc
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358923"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getTeamsDeviceUsageUserCounts = await graphClient.Reports
    .GetTeamsDeviceUsageUserCounts("D7")
    .Request()
    .GetAsync();

```