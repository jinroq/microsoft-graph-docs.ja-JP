---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: cb79352ec7ef88e182f0f40a7d2b673978386109
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891872"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetEmailActivityUserDetail('D7')
    .Request()
    .GetAsync();

```