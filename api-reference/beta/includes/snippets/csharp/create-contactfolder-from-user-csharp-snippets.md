---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4744ca346f9c6ad6b47a49d79f002dfcdb2fb0f0
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35486603"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contactFolder = new ContactFolder
{
    ParentFolderId = "parentFolderId-value",
    DisplayName = "displayName-value"
};

await graphClient.Me.ContactFolders
    .Request()
    .AddAsync(contactFolder);

```