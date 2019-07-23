---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b4c0145ef94b4c22d9c34aaa90bb923e43270e40
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35711859"
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
    SecurityEnabled = false
};

await graphClient.Groups
    .Request()
    .AddAsync(group);

```