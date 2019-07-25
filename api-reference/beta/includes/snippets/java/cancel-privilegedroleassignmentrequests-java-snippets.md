---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 78032cb24e9962dd801f37a84b197363dc461dbd
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875607"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.privilegedRoleAssignmentRequests("7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee")
    .cancel()
    .buildRequest()
    .post();

```