---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: cc23ce61c9a64e1474d25d8c0a4036eba7f48671
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35527153"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var columns = await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Columns
    .Request()
    .GetAsync();

```