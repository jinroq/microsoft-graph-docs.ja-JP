---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: be5a5c523727e3ad0b162f4aba5f1c2647ee8486
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35711499"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var applications = await graphClient.Applications
    .Request()
    .GetAsync();

```