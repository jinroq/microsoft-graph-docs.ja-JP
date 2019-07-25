---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d746a0334b66cc2234a97bd9a8fd6c93de2a3c26
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872888"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOffice365ActiveUserCounts = await graphClient.Reports
    .GetOffice365ActiveUserCounts('D7')
    .Request()
    .GetAsync();

```