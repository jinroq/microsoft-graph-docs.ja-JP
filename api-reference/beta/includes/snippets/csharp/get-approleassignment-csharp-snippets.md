---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e8d5d291c4d97f513e04353f49e21b1d755a8f27
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35710101"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appRoleAssignment = await graphClient.AppRoleAssignments["{id}"]
    .Request()
    .GetAsync();

```