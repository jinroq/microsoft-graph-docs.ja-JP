---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4d559851524c190907b9454449b511a336a2cd13
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35733341"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var profilePhoto = new ProfilePhoto
{
    Height = 99,
    Width = 99,
    Id = "id-value"
};

await graphClient.Users["{id|userPrincipalName}"].Photo
    .Request()
    .UpdateAsync(profilePhoto);

```