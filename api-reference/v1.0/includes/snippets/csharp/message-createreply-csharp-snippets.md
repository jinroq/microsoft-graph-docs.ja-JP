---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c8af78e00204174f338e505f418311229261b4bd
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35514286"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Messages["{id}"]
    .CreateReply()
    .Request()
    .PostAsync();

```