---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3783e4d3f5585c52b5b75b9ba9bc50460476de03
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35712507"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["11021"].Assignments["19002"].Submissions["850f51b7"]
    .Return()
    .Request()
    .PostAsync();

```