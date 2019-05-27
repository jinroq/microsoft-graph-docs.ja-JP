---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ef3e4b24b155f3322a01d3d8b99b991ce360e3bf
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34475281"
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