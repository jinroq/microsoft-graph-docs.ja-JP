---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: de4ece07df6e7bb8d93da7e328d8cf9c36d06eaa
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35496251"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetSkypeForBusinessPeerToPeerActivityUserCounts('D7')
    .Request()
    .GetAsync();

```