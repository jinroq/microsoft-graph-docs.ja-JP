---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: dde4b89f6986fb698d8b14a79ba9a2eef6fc0cc0
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35714301"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Users["13019"]
    .Request()
    .DeleteAsync();

```