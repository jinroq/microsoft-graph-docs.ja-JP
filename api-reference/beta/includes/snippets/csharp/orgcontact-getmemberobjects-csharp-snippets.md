---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ac1492e26eb8f9ee331926debb7111215dcca8ff
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35729043"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityEnabledOnly = true;

await graphClient.Contacts["{id}"]
    .GetMemberObjects(securityEnabledOnly)
    .Request()
    .PostAsync();

```