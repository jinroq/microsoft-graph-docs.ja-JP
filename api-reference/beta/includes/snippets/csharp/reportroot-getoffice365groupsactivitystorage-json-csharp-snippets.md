---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1e46a6ff6125d7901f4c4ca657808362331440bb
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36360399"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOffice365GroupsActivityStorage = await graphClient.Reports
    .GetOffice365GroupsActivityStorage("D7")
    .Request()
    .GetAsync();

```