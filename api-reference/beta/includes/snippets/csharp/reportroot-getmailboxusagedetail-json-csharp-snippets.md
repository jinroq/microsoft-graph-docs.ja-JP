---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 02cc20af9a1a092ed890ed883fdce86dae2c7a86
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36360575"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getMailboxUsageDetail = await graphClient.Reports
    .GetMailboxUsageDetail("D7")
    .Request()
    .GetAsync();

```