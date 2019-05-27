---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 05db449e89d98c30d065c682c2fc041fb00c5886
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34448147"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var orgContact = await graphClient.Contacts["{id}"]
    .Request()
    .GetAsync();

```