---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 87ea6a9955decfca7ce6cadec6c4e5b1c3e6e45d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35715546"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var members = await graphClient.Groups["{id}"].Members
    .Request()
    .GetAsync();

```