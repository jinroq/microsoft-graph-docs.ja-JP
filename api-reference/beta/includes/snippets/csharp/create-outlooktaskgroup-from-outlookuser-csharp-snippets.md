---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: af60d1a2fe413e0cfec526e39d17116425aa6c8c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35728806"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var outlookTaskGroup = new OutlookTaskGroup
{
    Name = "Leisure tasks"
};

await graphClient.Me.Outlook.TaskGroups
    .Request()
    .AddAsync(outlookTaskGroup);

```