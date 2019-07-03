---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a43245a951290d69d83ec643f9d8b12b29f04fdb
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35471295"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetYammerActivityUserCounts('D7')
    .Request()
    .GetAsync();

```