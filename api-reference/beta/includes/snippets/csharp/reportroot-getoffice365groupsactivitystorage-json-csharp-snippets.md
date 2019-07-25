---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 598cffaa494bf6c67c9e17ca9d691fed6c7c170b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873273"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOffice365GroupsActivityStorage = await graphClient.Reports
    .GetOffice365GroupsActivityStorage('D7')
    .Request()
    .GetAsync();

```