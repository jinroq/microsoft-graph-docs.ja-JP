---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 54fc34ec937d872a4328eba95e987f744c278edd
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35526236"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{teamId}"].Schedule.Shifts["{shiftId}"]
    .Request()
    .DeleteAsync();

```