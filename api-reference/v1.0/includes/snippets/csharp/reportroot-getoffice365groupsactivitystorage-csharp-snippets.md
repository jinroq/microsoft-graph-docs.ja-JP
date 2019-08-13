---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d3b0dad6693d675e8d6072812f05d2ebd7ad2b04
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36373619"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetOffice365GroupsActivityStorage("D7")
    .Request()
    .GetAsync();

```