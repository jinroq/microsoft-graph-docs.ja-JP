---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ea88dd497bff512531bfdf9fb5d635e520fabd08
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35495651"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = new Group
{
    Description = "description-value",
    DisplayName = "displayName-value",
    GroupTypes = new List<String>()
    {
        "groupTypes-value"
    },
    Mail = "mail-value",
    MailEnabled = true,
    MailNickname = "mailNickname-value"
};

await graphClient.Groups["{id}"]
    .Request()
    .UpdateAsync(group);

```