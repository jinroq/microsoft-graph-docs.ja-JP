---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9622f19c61681333d636b536dee00d4d5ebf32fe
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35730586"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var taskFolders = await graphClient.Me.Outlook.TaskFolders
    .Request()
    .GetAsync();

```