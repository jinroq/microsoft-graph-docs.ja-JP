---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0d7c58955b4fa98f0c3c9c460a423244f6c24be1
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35859063"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.privilegedAccess("azureResources").roleAssignmentRequests("7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee")
    .updateRequest(decision,assignmentState,schedule,reason)
    .buildRequest()
    .post();

```