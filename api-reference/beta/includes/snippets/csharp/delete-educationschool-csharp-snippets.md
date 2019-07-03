---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0933b3bcf9bdabc4026ba9a9c4c05d530e799dda
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35526010"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Schools["10002"]
    .Request()
    .DeleteAsync();

```