---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c8af78e00204174f338e505f418311229261b4bd
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34455454"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Messages["{id}"]
    .CreateReply()
    .Request()
    .PostAsync();

```