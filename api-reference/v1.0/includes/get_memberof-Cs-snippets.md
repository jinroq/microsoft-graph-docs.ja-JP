---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b4b0dc4cc0c2aeaa733c0b5f7f0429527261ace0
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34477753"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var memberOf = await graphClient.Me.MemberOf
    .Request()
    .GetAsync();

```