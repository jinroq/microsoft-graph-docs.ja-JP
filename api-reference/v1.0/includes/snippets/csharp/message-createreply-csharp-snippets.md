---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c8af78e00204174f338e505f418311229261b4bd
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35732200"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Messages["{id}"]
    .CreateReply()
    .Request()
    .PostAsync();

```