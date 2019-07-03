---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 054336833d11d1d6e5ac5cfadb5a55f2dc4b6b7b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35527081"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookNamedItem = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"]
    .Request()
    .GetAsync();

```