---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b7877ea77f412edbea4ec16e8bf631caa167455a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35710886"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.AccessReviews["2975E9B5-44CE-4E71-93D3-30F03B5AA992"]
    .ResetDecisions()
    .Request()
    .PostAsync();

```