---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b647a50659bb2e239c1306d2d3a65adbbe2feed6
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35495602"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetSharePointSiteUsagePages('D7')
    .Request()
    .GetAsync();

```