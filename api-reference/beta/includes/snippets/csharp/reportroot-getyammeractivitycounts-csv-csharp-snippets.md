---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1dcacca897ea1a976df260c7ceb374c9f0b57ae9
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358683"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getYammerActivityCounts = await graphClient.Reports
    .GetYammerActivityCounts("D7")
    .Request()
    .GetAsync();

```