---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8d26ca1824c4bcf3d67925a51ec8f4863f221786
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35464449"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Agreements["'id'"]
    .Request()
    .DeleteAsync();

```