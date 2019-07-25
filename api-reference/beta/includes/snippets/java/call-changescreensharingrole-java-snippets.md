---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d27e9797bbcee5f47a82c04c1a31e56c00e4c0e5
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35864855"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ScreenSharingRole role = ScreenSharingRole.VIEWER;

graphClient.app().calls("{id}")
    .changeScreenSharingRole(role)
    .buildRequest()
    .post();

```