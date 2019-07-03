---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 52edce7be4867baa2710b6d69a7cf3fa44b21a9a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35486807"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var domains = await graphClient.Domains
    .Request()
    .GetAsync();

```