---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: cea3d85ae902585f5a306c045e7685345a7c48fe
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34437931"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Messages["AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==="].Extensions["Com.Contoso.Referral"]
    .Request()
    .DeleteAsync();

```