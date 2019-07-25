---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d967303bbd02982f4e41e1810779d1724f41961a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871203"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var credentialUserRegistrationDetails = await graphClient.Reports.CredentialUserRegistrationDetails
    .Request()
    .GetAsync();

```