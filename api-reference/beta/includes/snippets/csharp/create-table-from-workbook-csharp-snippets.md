---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5abcf407f9c89364a8a7b4f5c199a719f4e79845
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35723806"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var address = "A1:D8";

var hasHeaders = false;

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables
    .Add(address,hasHeaders)
    .Request()
    .PostAsync();

```