---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 891d096529d43d7de87fca307bb926c791f9fdc8
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35717974"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sectionGroup = await graphClient.Me.Onenote.SectionGroups["{id}"]
    .Request()
    .GetAsync();

```