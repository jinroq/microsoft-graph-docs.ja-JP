---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6da78a6366f5337ff0b348d141c1c506dcae6f5b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35705718"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["11021"].Assignments["19002"].Resources["22002"]
    .Request()
    .DeleteAsync();

```