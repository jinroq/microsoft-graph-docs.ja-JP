---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 25c3f9dd496c2a2bb6eee627a0d0b5b8b9788ca0
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35514121"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var licenseDetails = await graphClient.Me.LicenseDetails
    .Request()
    .GetAsync();

```