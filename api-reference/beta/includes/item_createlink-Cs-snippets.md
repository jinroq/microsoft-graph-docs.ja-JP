---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2a2136af5fae87c1a643ddd35a2cd670cd021915
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34444553"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var type = "view";

var scope = "anonymous";

await graphClient.Me.Drive.Items["{itemId}"]
    .CreateLink(type,scope,expirationDateTime,password,message,recipients)
    .Request()
    .PostAsync();

```