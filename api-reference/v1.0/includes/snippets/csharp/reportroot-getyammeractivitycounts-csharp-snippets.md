---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8d97904f7dade188938e4269829c3a6f2a242340
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320401"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetYammerActivityCounts("D7")
    .Request()
    .GetAsync();

```