---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0c91d18cd05ea68dba69f8473be110e8e62658e2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35471851"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var type = "edit";

var scope = "organization";

await graphClient.Me.Drive.Items["{item-id}"]
    .CreateLink(type,scope)
    .Request()
    .PostAsync();

```