---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a2efd22c8f11bf00157bc160bc9842603d874c84
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35859050"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GovernanceRoleSetting governanceRoleSetting = graphClient.privilegedAccess("azureResources").roleSettings("80dc5d6f-8d89-47b3-953f-01dc909ed3f9")
    .buildRequest()
    .get();

```