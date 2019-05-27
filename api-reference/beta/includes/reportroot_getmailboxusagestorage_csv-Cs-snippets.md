---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a52b317178c7c501d76b6c77ffffd9a91b45937f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34441893"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getMailboxUsageStorage = await graphClient.Reports.GetMailboxUsageStorage('D7')
    .Request()
    .GetAsync();

```