---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 68b248900b57b6164937f3b569fa5d2bb0c62470
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35707677"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var hostedContents = await graphClient.Chats["{id}"].Messages["{id}"].HostedContents
    .Request()
    .GetAsync();

```