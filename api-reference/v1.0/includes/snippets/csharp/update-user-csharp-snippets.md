---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 64f3465f2cca9a803587aec82f5a86b32e439e67
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35513474"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var user = new User
{
    AccountEnabled = true,
    BusinessPhones = new List<String>()
    {
        "businessPhones-value"
    },
    City = "city-value"
};

await graphClient.Me
    .Request()
    .UpdateAsync(user);

```