---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f9d9a2b4c76fdcb2186000da275c2eab35b04d77
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320672"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSkypeForBusinessParticipantActivityMinuteCounts("D7")
    .Request()
    .GetAsync();

```