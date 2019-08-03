---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: cbeeeb840080e9e465b0fda2e38ef7123a8d6c13
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173006"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var featureRolloutPolicies = await graphClient.Directory.FeatureRolloutPolicies
    .Request()
    .GetAsync();

```