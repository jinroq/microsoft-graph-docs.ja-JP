---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 62c6d0e7a1356efe68e04fa2867737c6da1cce53
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35526311"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{id|userPrincipalName}"].Photo
    .Request()
    .DeleteAsync();

```