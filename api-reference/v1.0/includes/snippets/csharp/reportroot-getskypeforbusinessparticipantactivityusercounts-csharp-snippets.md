---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2c1236e99ce1a59cdb909a440749119c29888e4d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320679"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSkypeForBusinessParticipantActivityUserCounts("D7")
    .Request()
    .GetAsync();

```