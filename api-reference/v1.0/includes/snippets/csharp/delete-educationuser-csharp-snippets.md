---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a0a350786874bb7faea8c5d040cdf7fd3e430541
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35732752"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Users["{user-id}"]
    .Request()
    .DeleteAsync();

```