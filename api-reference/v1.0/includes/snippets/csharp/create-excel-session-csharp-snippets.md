---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5b8cb8f5fa1c29c3946255ebb311adaceec70c12
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36365572"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var persistChanges = true;

await graphClient.Me.Drive.Items["{id}"].Workbook
    .CreateSession(persistChanges)
    .Request()
    .PostAsync();

```