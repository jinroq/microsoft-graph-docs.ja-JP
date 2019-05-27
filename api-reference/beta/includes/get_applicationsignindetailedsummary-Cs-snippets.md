---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3b0d05b4c0a9df13a0ae16d56704747a4d30a07d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34474038"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var applicationSignInDetailedSummary = await graphClient.Reports.ApplicationSignInDetailedSummary["'id'"]
    .Request()
    .GetAsync();

```