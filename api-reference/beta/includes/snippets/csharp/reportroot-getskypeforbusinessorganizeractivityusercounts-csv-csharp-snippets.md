---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1c14a789bf73c3a88cd22a58f9068edf627632a1
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359228"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSkypeForBusinessOrganizerActivityUserCounts = await graphClient.Reports
    .GetSkypeForBusinessOrganizerActivityUserCounts("D7")
    .Request()
    .GetAsync();

```