---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: aa24f2a23e735bded2d1d48f0c4a682933104104
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359041"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSkypeForBusinessPeerToPeerActivityCounts = await graphClient.Reports
    .GetSkypeForBusinessPeerToPeerActivityCounts("D7")
    .Request()
    .GetAsync();

```