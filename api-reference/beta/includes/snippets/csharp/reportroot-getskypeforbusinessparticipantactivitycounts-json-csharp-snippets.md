---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: dc20184dd4fe7efe8fa5d5dcec2f06d84dc5ce03
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359187"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSkypeForBusinessParticipantActivityCounts = await graphClient.Reports
    .GetSkypeForBusinessParticipantActivityCounts("D7")
    .Request()
    .GetAsync();

```