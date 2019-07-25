---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4d53196e7e602f2f90183c5e95d8206bacf57c33
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35710569"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var agreement = await graphClient.Agreements["'id'"]
    .Request()
    .Expand("files")
    .GetAsync();

```