---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: dee8989e645d157a0e173e9ae2330902266fb672
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35735679"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.DirectoryObjects["{id}"]
    .Request()
    .DeleteAsync();

```