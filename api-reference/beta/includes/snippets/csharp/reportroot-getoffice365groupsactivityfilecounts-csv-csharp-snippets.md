---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 50a76312472d69bab106ef5e8bcc8a5e86d442f6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36360394"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOffice365GroupsActivityFileCounts = await graphClient.Reports
    .GetOffice365GroupsActivityFileCounts("D7")
    .Request()
    .GetAsync();

```