---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b386aa3d0d58bdde4f49d255d3f55ef16b1f589c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36325845"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook
    .RefreshSession()
    .Request()
    .Header("workbook-session-id","{session-id}")
    .PostAsync();

```