---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8595c9db837753828059e3b4fb79710b7cd02073
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871231"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userCredentialUsageDetails = await graphClient.Reports.UserCredentialUsageDetails
    .Request()
    .GetAsync();

```