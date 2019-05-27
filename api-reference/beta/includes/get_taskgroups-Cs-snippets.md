---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ca8f9d87ce0baa79b2201c283a2080a881a3dd9c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34445435"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var taskGroups = await graphClient.Me.Outlook.TaskGroups
    .Request()
    .GetAsync();

```