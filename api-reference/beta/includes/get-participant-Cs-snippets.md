---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 76f36a3dee42a6fb5619e25c551f3e48ffec8393
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34435936"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var Participant = await graphClient.App.Calls["{id}"].Participants["{id}"]
    .Request()
    .GetAsync();

```