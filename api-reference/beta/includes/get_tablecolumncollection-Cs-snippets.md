---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: cc23ce61c9a64e1474d25d8c0a4036eba7f48671
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34445638"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var columns = await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Columns
    .Request()
    .GetAsync();

```