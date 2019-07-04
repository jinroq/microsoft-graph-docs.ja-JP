---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 711e0ffeabd73b0ce6c8873fc4da7bd394f7bb39
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35533533"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var user = await graphClient.Users["{user-id}"]
    .Request()
    .GetAsync();

```