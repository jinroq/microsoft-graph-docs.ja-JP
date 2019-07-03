---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 891d096529d43d7de87fca307bb926c791f9fdc8
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35513872"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sectionGroup = await graphClient.Me.Onenote.SectionGroups["{id}"]
    .Request()
    .GetAsync();

```