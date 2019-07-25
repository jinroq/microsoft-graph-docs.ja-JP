---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 762704527d002291e1012a30651f7712933a0977
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35710673"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var administrativeUnits = await graphClient.AdministrativeUnits
    .Request()
    .GetAsync();

```