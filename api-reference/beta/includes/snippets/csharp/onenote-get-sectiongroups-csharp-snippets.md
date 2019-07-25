---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fd4e873873491ea2465fa029e505145f389e5646
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878874"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sectionGroups = await graphClient.Me.Onenote.SectionGroups
    .Request()
    .GetAsync();

```