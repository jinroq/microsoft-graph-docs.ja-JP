---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4a7367dd63b34c9c530ed27985cfa1cb7335fdfa
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35720794"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var outlookTaskFolder = new OutlookTaskFolder
{
    Name = "Volunteer"
};

await graphClient.Me.Outlook.TaskFolders
    .Request()
    .AddAsync(outlookTaskFolder);

```