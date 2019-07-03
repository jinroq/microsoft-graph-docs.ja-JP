---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8632a3ca72576a0eb24005cc6389c76e87279c1d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35513627"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var registeredDevices = await graphClient.Me.RegisteredDevices
    .Request()
    .GetAsync();

```