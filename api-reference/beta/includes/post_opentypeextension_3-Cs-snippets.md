---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b96e48dcc26de546bbf86fb7115dccf052cbdee6
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/29/2019
ms.locfileid: "34546797"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var extension = new Extension
{
    ExtensionName = "Com.Contoso.Deal",
    CompanyName = "Alpine Skis",
    DealValue = 1010100,
    ExpirationDate = "2015-07-03T13:04:00Z"
};

await graphClient.Groups["f5480dfd-7d77-4d0b-ba2e-3391953cc74a"].Events["AAMkADVl17IsAAA="].Extensions
    .Request()
    .AddAsync(extension);

```