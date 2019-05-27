---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7bbf4c4abb00a839a61450856f3e3aecffe01be6
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34441592"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOffice365ActiveUserDetail = await graphClient.Reports.GetOffice365ActiveUserDetail('D7')
    .Request()
    .GetAsync();

```