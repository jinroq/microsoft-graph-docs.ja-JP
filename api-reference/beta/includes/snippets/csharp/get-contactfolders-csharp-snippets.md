---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c1b15df1afa9e870eb6291109af2e1c7dbfeb8ee
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724206"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contactFolders = await graphClient.Me.ContactFolders
    .Request()
    .GetAsync();

```