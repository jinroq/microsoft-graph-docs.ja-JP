---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b249f129d0cfad1de47396fc88e030a5cb591821
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932511"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var displayName = "Myprefix_test_mysuffix";

var mailNickname = "Myprefix_test_mysuffix";

var onBehalfOfUserId = "onBehalfOfUserId-value";

await graphClient.Groups["{id}"]
    .ValidateProperties(displayName,mailNickname,onBehalfOfUserId)
    .Request()
    .PostAsync();

```