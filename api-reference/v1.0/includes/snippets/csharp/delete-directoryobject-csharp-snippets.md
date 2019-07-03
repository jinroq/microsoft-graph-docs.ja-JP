---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: dee8989e645d157a0e173e9ae2330902266fb672
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35471977"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.DirectoryObjects["{id}"]
    .Request()
    .DeleteAsync();

```