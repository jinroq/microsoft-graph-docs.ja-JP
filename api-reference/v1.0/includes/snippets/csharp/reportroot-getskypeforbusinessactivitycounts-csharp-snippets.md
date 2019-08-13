---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 34e4487543be32379cae8387d68ed46f7f4997d5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349337"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSkypeForBusinessActivityCounts("D7")
    .Request()
    .GetAsync();

```