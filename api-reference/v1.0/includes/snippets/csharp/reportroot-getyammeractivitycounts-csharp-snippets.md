---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c43bc08cc299683ce64bde6756f6789e64311893
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35738037"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetYammerActivityCounts('D7')
    .Request()
    .GetAsync();

```