---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 423a5696e3c02c58e904b54b5fd03832941c1ae3
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/11/2019
ms.locfileid: "36846115"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var administrativeUnit = new AdministrativeUnit
{
    DisplayName = "Seattle District Technical Schools",
    Description = "Seattle district technical schools administration",
    Visibility = true
};

await graphClient.AdministrativeUnits
    .Request()
    .AddAsync(administrativeUnit);

```