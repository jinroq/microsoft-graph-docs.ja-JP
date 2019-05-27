---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 23db8bf9f3dbe6662f430e02d8106c5199bca6a3
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34474395"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessReview = await graphClient.AccessReviews["2b83cc42-09db-46f6-8c6e-16fec466a82d"]
    .Request()
    .GetAsync();

```