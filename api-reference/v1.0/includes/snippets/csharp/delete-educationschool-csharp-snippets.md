---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b6fa6bcf334d47b90b18e90969d049bf19672292
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35735638"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Schools["{school-id}"]
    .Request()
    .DeleteAsync();

```