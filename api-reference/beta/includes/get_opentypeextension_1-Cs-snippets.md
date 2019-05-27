---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d5a410f45520840b68c291a6ca72748015c1d0c0
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34448273"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var extension = await graphClient.Me.Messages["AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==='"].Extensions["Com.Contoso.Referral"]
    .Request()
    .GetAsync();

```