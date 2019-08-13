---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 074923f5b10d540b32168bb3c97b32a5626d95cf
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359694"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSharePointSiteUsageDetail = await graphClient.Reports
    .GetSharePointSiteUsageDetail("D7")
    .Request()
    .GetAsync();

```