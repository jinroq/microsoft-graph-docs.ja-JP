---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a446c19fcbcf6ea95976171668cf06129ed32069
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35884663"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetOffice365GroupsActivityFileCounts('D7')
    .Request()
    .GetAsync();

```