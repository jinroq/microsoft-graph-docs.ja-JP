---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 791ff036fd126621b2820653633f01f25b3f8710
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35740943"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contactFolder = new ContactFolder
{
    DisplayName = "displayName-value"
};

await graphClient.Me.ContactFolders["{id}"].ChildFolders
    .Request()
    .AddAsync(contactFolder);

```