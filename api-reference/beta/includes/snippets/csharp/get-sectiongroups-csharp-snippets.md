---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0d3ed7b57d2beec92bfa0426168c9cea33c0618f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35727453"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sectionGroups = await graphClient.Me.Onenote.SectionGroups["{id}"].SectionGroups
    .Request()
    .GetAsync();

```