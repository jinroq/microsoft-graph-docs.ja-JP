---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ca8f9d87ce0baa79b2201c283a2080a881a3dd9c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35728835"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var taskGroups = await graphClient.Me.Outlook.TaskGroups
    .Request()
    .GetAsync();

```