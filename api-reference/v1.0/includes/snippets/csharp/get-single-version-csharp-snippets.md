---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 25f544146d6dcf1f7fc01e497bdb4c0a51945468
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35730765"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItemVersion = await graphClient.Me.Drive.Items["{item-id}"].Versions["{version-id}"]
    .Request()
    .GetAsync();

```