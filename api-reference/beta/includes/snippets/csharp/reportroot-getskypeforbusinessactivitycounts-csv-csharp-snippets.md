---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fc48b798e83f57c199842ec69c5c0fa7db1b250c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359637"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSkypeForBusinessActivityCounts = await graphClient.Reports
    .GetSkypeForBusinessActivityCounts("D7")
    .Request()
    .GetAsync();

```