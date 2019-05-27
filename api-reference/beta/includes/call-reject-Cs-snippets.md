---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3cd71ac033bd0b1be817f06b53c7f70c91f11c8f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34456222"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var reason = "none";

await graphClient.App.Calls["{id}"]
    .Reject(reason)
    .Request()
    .PostAsync();

```