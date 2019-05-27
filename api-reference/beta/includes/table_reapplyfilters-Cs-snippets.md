---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a30ec7733186ae4cd6c83ff0ebf4a842862c96cc
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34465875"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"]
    .ReapplyFilters()
    .Request()
    .PostAsync();

```