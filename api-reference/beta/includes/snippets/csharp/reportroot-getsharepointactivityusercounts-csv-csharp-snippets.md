---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5fca14303b3efa9f5cf48576fbc0a4c86b9e7de7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359854"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSharePointActivityUserCounts = await graphClient.Reports
    .GetSharePointActivityUserCounts("D7")
    .Request()
    .GetAsync();

```