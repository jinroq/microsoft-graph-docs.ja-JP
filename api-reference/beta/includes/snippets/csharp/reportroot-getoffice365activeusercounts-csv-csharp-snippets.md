---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 365b64a8f5e03f8a5260aec9163392ce7dfb148a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36360465"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOffice365ActiveUserCounts = await graphClient.Reports
    .GetOffice365ActiveUserCounts("D7")
    .Request()
    .GetAsync();

```