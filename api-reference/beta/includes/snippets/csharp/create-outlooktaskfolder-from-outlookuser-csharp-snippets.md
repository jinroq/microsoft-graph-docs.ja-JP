---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4a7367dd63b34c9c530ed27985cfa1cb7335fdfa
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35526024"
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