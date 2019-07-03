---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a611c46b3ad31de89c746e1d473f8d1bf9fff969
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35495610"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetSharePointActivityUserCounts('D7')
    .Request()
    .GetAsync();

```