---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 24d3b28bb12c00f65ab44d6ead523e069a16a496
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725774"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var riskDetections = await graphClient.RiskDetections
    .Request()
    .Filter("riskType eq 'unfamiliarFeatures' or riskLevel eq 'medium'")
    .GetAsync();

```