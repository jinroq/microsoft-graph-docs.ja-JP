---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2e5fb25135bb6a298a6a3be78e6096dc3bcfe7f3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35887704"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var users = await graphClient.Education.Schools["{school-id}"].Users
    .Request()
    .GetAsync();

```