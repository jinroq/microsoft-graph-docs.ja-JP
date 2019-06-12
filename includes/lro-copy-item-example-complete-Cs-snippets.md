---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: dc93bcaf0755ac9776f4e88ea0c754c09245f975
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34843711"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = await graphClient.Me.Drive.Items["{item-id}"]
    .Request()
    .GetAsync();

```