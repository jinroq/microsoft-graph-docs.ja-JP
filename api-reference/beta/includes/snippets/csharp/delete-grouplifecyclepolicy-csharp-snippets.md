---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d6b6fef0b4ed19651c0f3fad7c659a6e104279aa
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35705423"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.GroupLifecyclePolicies["{id}"]
    .Request()
    .DeleteAsync();

```