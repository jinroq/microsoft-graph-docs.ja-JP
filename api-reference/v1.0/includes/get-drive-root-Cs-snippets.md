---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fc3e4d190cc84edc7be903228c5d9d8bb10cfb10
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34454931"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = await graphClient.Me.Drive.Root
    .Request()
    .GetAsync();

```