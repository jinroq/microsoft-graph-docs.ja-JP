---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 795a047824a0f5ca7b593a65ebec5d8bdd895861
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34477167"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetSharePointActivityUserDetail('D7')
    .Request()
    .GetAsync();

```