---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8a2e624a82fd1e3c7fe9eedbbf2250a8da2f1bba
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35736820"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].UsedRange()
    .Request()
    .GetAsync();

```