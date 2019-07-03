---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c0cc58c05aee4a7cd0098a5fec79c0987ef0f1a3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35527663"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getYammerActivityCounts = await graphClient.Reports.GetYammerActivityCounts('D7')
    .Request()
    .GetAsync();

```