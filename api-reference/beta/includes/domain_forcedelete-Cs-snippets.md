---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 18ba187c8620a57cbe4d9c868d421eda73f915a2
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34437091"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var disableUserAccounts = true;

await graphClient.Domains["contoso.com"]
    .ForceDelete(disableUserAccounts)
    .Request()
    .PostAsync();

```