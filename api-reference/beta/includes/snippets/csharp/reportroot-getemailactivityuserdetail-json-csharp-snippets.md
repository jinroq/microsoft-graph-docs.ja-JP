---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6ebc9f55e08ee1a88e52416b0ba51a94c2128071
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36308506"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getEmailActivityUserDetail = await graphClient.Reports
    .GetEmailActivityUserDetail("D7")
    .Request()
    .GetAsync();

```