---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8674dd49aaa6d4a7d3251a15f1f9efeee025160b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35860945"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var search = await graphClient.Me.Drive
    .Search('{search-query}')
    .Request()
    .GetAsync();

```