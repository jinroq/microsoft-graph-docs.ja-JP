---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 778a54e4abb7332f4b476448479353ac8482df48
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891816"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetEmailActivityUserCounts('D7')
    .Request()
    .GetAsync();

```