---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6a74871dcc0ac5c9d6ca8128b3cf59e16de958d0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36308765"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getCredentialUsageSummary = await graphClient.Reports
    .GetCredentialUsageSummary("D30")
    .Request()
    .Filter("feature eq 'registration'")
    .GetAsync();

```