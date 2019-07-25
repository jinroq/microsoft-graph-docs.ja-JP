---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f429b8c1a671530d6fbddcfdc86c2769f6d9a0ff
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873995"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getEmailActivityUserDetail = await graphClient.Reports
    .GetEmailActivityUserDetail('D7')
    .Request()
    .GetAsync();

```