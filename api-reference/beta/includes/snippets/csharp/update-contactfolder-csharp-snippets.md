---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ef3e4b24b155f3322a01d3d8b99b991ce360e3bf
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35526558"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contactFolder = new ContactFolder
{
    ParentFolderId = "parentFolderId-value",
    DisplayName = "displayName-value"
};

await graphClient.Me.ContactFolders["{id}"]
    .Request()
    .UpdateAsync(contactFolder);

```