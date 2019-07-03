---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 73cfc36775de434ec6596e60e8157dae4b602680
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35527266"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getEmailAppUsageUserDetail = await graphClient.Reports.GetEmailAppUsageUserDetail('D7')
    .Request()
    .GetAsync();

```