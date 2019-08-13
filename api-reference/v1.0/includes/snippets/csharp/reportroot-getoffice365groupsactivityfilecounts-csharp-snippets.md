---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e435e002f72e43725fa63918d0c89932c75d3b91
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36373724"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetOffice365GroupsActivityFileCounts("D7")
    .Request()
    .GetAsync();

```