---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a80f100adcf65736815703c425d1eeab72f67027
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35526838"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOffice365ServicesUserCounts = await graphClient.Reports.GetOffice365ServicesUserCounts('D7')
    .Request()
    .GetAsync();

```