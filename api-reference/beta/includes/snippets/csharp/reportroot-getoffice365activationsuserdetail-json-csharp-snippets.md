---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7ffb1d3678ade75070a5e3c6114867d38324e90e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873526"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOffice365ActivationsUserDetail = await graphClient.Reports
    .GetOffice365ActivationsUserDetail()
    .Request()
    .GetAsync();

```