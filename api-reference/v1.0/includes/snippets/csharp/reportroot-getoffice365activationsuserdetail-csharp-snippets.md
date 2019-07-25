---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8decb00c9c96188936a22d4da727128dd2acba99
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881057"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetOffice365ActivationsUserDetail()
    .Request()
    .GetAsync();

```