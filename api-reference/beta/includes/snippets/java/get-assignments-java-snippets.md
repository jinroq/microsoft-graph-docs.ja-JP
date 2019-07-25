---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 384cef0dbbc1a69c32256523d8ab65f3e95c74c5
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875851"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPrivilegedRoleAssignmentCollectionPage assignments = graphClient.privilegedRoles("{id}").assignments()
    .buildRequest()
    .get();

```