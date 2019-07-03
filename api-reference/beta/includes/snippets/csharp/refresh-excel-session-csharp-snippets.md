---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a37fccafdc8707fd5635da7b2cfb97f9fe54440b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35486467"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook
    .RefreshSession(this)
    .Request()
    .Header("workbook-session-id","{session-id}")
    .PostAsync();

```