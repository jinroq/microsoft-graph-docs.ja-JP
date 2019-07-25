---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ade9452388a76649cbaee0a1e55321f8298bf894
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35858792"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Groups
    .Delta()
    .Request()
    .GetAsync();

```