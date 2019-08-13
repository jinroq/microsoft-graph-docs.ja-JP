---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8ebb2c0da32a0b0309b03ab68bf02f6e4ac1b851
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36331227"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var user = await graphClient.Education.Me.User
    .Request()
    .GetAsync();

```