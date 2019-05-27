---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 881e643f93eddc41593d8db5d8c14cc3a8654b1d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34468478"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetEmailActivityUserDetail('D7')
    .Request()
    .GetAsync();

```