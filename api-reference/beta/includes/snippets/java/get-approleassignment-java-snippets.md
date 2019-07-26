---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: bb93e5c41be38c7bd54ce0dbad42e4891825c4ec
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856651"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AppRoleAssignment appRoleAssignment = graphClient.appRoleAssignments("{id}")
    .buildRequest()
    .get();

```