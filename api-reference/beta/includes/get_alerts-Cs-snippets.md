---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7bf07cb98320e2f06b14a844161a67289bb8ffff
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34474122"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var alerts = await graphClient.Security.Alerts
    .Request()
    .GetAsync();

```