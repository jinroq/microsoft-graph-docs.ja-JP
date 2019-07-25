---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9736f77673ba3109534e651a587fd3641c173d5b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35715678"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var devices = await graphClient.Devices
    .Request()
    .GetAsync();

```