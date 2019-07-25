---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 939dafdfa2983ee68ebb771a3b75a8d3bb465a08
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35734061"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityEnabledOnly = true;

await graphClient.DirectoryObjects["{object-id}"]
    .GetMemberObjects(securityEnabledOnly)
    .Request()
    .PostAsync();

```