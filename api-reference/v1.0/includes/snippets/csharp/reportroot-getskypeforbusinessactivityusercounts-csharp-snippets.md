---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 749fd8d5cf736bd83ffc718cb78029eabdd14d5d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35495592"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetSkypeForBusinessActivityUserCounts('D7')
    .Request()
    .GetAsync();

```