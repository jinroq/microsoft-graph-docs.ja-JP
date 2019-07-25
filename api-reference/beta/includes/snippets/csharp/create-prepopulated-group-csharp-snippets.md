---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1e355248684978c4832670fc948f9339669aebfb
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35858158"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = new Group
{
    Description = "Group with designated owner and members",
    DisplayName = "Operations group",
    GroupTypes = new List<String>()
    {
        "Unified"
    },
    MailEnabled = true,
    MailNickname = "operations2019",
    SecurityEnabled = false,
    AdditionalData = new Dictionary<string, object>()
    {
        {"members@odata.bind",["https://graph.microsoft.com/beta/users/ff7cb387-6688-423c-8188-3da9532a73cc","https://graph.microsoft.com/beta/users/69456242-0067-49d3-ba96-9de6f2728e14"]},
        {"owners@odata.bind",["https://graph.microsoft.com/beta/users/26be1845-4119-4801-a799-aea79d09f1a2"]}
    }
};

await graphClient.Groups
    .Request()
    .AddAsync(group);

```