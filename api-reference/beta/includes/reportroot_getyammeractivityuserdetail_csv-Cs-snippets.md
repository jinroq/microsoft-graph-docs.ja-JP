---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 627a877b6da9510b772424eecc738492f4a4963c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34452701"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getYammerActivityUserDetail = await graphClient.Reports.GetYammerActivityUserDetail('D7')
    .Request()
    .GetAsync();

```