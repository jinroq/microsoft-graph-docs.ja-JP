---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1fc6dc4c1bf0eb2e7162b4c6e49ca952466d0a11
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893540"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSharePointActivityUserCounts('D7')
    .Request()
    .GetAsync();

```