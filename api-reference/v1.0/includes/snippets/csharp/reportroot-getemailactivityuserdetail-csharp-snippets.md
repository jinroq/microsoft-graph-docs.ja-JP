---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 608a65599ed905c4e36466db4f1ab2c223b50c73
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327405"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetEmailActivityUserDetail("D7")
    .Request()
    .GetAsync();

```