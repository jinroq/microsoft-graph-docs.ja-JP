---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1ce0ebf0e7f3d82ac6a6c81852ee67e816a13979
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359143"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSkypeForBusinessParticipantActivityMinuteCounts = await graphClient.Reports
    .GetSkypeForBusinessParticipantActivityMinuteCounts("D7")
    .Request()
    .GetAsync();

```