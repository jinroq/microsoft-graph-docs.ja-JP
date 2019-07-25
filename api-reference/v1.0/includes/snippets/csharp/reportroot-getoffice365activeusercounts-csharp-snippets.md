---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 93469943f7902e02ec0c781ead39a6d2c34b47d5
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35890773"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetOffice365ActiveUserCounts('D7')
    .Request()
    .GetAsync();

```