---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 95061fa350a4a7497da2f1277b3642ace5cfaaf7
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35740880"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = await graphClient.Directory.DeletedItems["{object-id}"]
    .Request()
    .GetAsync();

```