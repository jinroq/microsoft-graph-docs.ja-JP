---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a30ec7733186ae4cd6c83ff0ebf4a842862c96cc
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35731739"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"]
    .ReapplyFilters()
    .Request()
    .PostAsync();

```