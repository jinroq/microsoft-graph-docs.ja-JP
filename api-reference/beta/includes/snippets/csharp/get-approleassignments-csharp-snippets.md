---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8803e13de770f6c692ef0da4cb605774cbc26ce0
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725319"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appRoleAssignments = await graphClient.ServicePrincipals["{id}"].AppRoleAssignments
    .Request()
    .GetAsync();

```