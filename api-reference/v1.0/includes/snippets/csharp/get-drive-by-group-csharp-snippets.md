---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 35dc3d56a2e44a371657d36d373bb486ce3b30d1
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35736477"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var drive = await graphClient.Groups["{groupId}"].Drive
    .Request()
    .GetAsync();

```