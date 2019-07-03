---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 74af7cd688d894c294fcfcbaac4998d49377ba2c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35513470"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var Stream = "The contents of the file goes here."

await graphClient.Me.Drive.Items["{item-id}"]
    .Request()
    .PutAsync(Stream);

```