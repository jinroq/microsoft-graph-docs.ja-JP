---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3626efc4092355e9aede2f8bc40e4bf6786bd193
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873231"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOffice365ServicesUserCounts = await graphClient.Reports
    .GetOffice365ServicesUserCounts('D7')
    .Request()
    .GetAsync();

```