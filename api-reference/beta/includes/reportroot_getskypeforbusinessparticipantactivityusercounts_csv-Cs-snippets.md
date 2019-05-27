---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c9289cec5e9d4b18a11dcad7fcaee45017eeef23
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34463996"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSkypeForBusinessParticipantActivityUserCounts = await graphClient.Reports.GetSkypeForBusinessParticipantActivityUserCounts('D7')
    .Request()
    .GetAsync();

```