---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1f64f7710ba9936492302cdc1fe46059a41bba37
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/11/2019
ms.locfileid: "36846108"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.App.Calls["57dab8b1-894c-409a-b240-bd8beae78896"]
    .Request()
    .DeleteAsync();

```