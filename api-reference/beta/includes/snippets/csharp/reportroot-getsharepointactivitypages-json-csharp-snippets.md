---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 59e4a39f5f8e58ed1d3251c38cd81b87c7434e78
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872848"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSharePointActivityPages = await graphClient.Reports
    .GetSharePointActivityPages('D7')
    .Request()
    .GetAsync();

```