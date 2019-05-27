---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 17354694f582e1439f3078a7b9ec85823350b9d6
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34480163"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userIds = new List<String>()
{
    "29f270bb-4d23-4f68-8a57-dc73dc0d4caf",
    "20f91ec9-d140-4d90-9cd9-f618587a1471"
};

await graphClient.RiskyUsers
    .ConfirmCompromised(userIds)
    .Request()
    .PostAsync();

```