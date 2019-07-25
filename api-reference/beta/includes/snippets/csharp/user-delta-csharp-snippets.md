---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f8e7b57fd79cbe7fd484584ccbdd97c53068e694
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867835"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Users
    .Delta()
    .Request()
    .GetAsync();

```