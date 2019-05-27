---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: be650d47890c14e974c31c6164137a3a2fa7b7e9
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34478740"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetOffice365GroupsActivityDetail('D7')
    .Request()
    .GetAsync();

```