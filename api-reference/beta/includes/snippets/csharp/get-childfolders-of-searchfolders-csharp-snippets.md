---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0948b00d09234f10da6195edbe21d7b64d9a36ee
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35486694"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var childFolders = await graphClient.Me.MailFolders["searchfolders"].ChildFolders
    .Request()
    .GetAsync();

```