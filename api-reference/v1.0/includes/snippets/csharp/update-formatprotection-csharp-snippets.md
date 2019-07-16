---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3d98fc1317500d7342fd99fe930198b50a11e862
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35740229"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookFormatProtection = new WorkbookFormatProtection
{
    Locked = true,
    FormulaHidden = true
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"].Range().Format.Protection
    .Request()
    .UpdateAsync(workbookFormatProtection);

```