---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f1ea6558a7c7f204e260fd6b1291edc17c47c4fd
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35894217"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Rows["{index}"]
    .Range()
    .Request()
    .GetAsync();

```