---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fef5d47afa3c85d1e5eb981ddc2f1d8fe280eba8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359761"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSharePointSiteUsageSiteCounts = await graphClient.Reports
    .GetSharePointSiteUsageSiteCounts("D7")
    .Request()
    .GetAsync();

```