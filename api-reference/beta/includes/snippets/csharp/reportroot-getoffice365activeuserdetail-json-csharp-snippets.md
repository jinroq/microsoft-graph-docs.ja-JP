---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 17c2608b7edf9e462a684b9ba66cef7cbacbc96e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36360517"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOffice365ActiveUserDetail = await graphClient.Reports
    .GetOffice365ActiveUserDetail("D7")
    .Request()
    .GetAsync();

```