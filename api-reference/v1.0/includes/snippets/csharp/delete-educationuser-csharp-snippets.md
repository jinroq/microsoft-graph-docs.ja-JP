---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a0a350786874bb7faea8c5d040cdf7fd3e430541
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35472494"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Users["{user-id}"]
    .Request()
    .DeleteAsync();

```