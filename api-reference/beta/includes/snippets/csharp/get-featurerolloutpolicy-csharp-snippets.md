---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6df23739610b7b82f116e5d0d647329bbfae086c
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/03/2019
ms.locfileid: "36172851"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var featureRolloutPolicy = await graphClient.Directory.FeatureRolloutPolicies["df85e4d9-e8c4-4033-a41c-73419a95c29c"]
    .Request()
    .Expand("appliesTo")
    .GetAsync();

```