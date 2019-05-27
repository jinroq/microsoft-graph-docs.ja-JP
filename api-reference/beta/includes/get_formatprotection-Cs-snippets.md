---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9c5ed53458a48b04fc1543c7fe146049cfe82afc
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34471216"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookFormatProtection = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"].Range().Format.Protection
    .Request()
    .GetAsync();

```