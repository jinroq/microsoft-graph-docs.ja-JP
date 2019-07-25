---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1a318a89b64f83f81dadb5b1a8d26bbf764fe2f7
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869986"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var owners = await graphClient.ServicePrincipals["{id}"].Owners
    .Request()
    .GetAsync();

```