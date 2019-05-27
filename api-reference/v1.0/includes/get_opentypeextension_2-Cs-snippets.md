---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1b7723a6b564b34551c1ee4f91bf2a5ae3d02b7c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34477391"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var extension = await graphClient.Groups["f5480dfd-7d77-4d0b-ba2e-3391953cc74a"].Events["AAMkADVl17IsAAA="].Extensions["Com.Contoso.Deal"]
    .Request()
    .GetAsync();

```