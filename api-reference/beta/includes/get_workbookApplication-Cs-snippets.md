---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 441bd7dc497bd2af2ae48b1d083109bb43f0c98f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34445134"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookApplication = await graphClient.Me.Drive.Items["{id}"].Workbook.Application
    .Request()
    .GetAsync();

```