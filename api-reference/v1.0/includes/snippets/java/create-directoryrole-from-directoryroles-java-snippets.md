---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a7ce4c28e517a1f1db161bcb7a61e3a12339f087
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865896"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryRole directoryRole = new DirectoryRole();
directoryRole.roleTemplateId = "roleTemplateId-value";

graphClient.directoryRoles()
    .buildRequest()
    .post(directoryRole);

```