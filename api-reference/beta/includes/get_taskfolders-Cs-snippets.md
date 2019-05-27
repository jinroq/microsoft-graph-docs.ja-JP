---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9622f19c61681333d636b536dee00d4d5ebf32fe
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34445505"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var taskFolders = await graphClient.Me.Outlook.TaskFolders
    .Request()
    .GetAsync();

```