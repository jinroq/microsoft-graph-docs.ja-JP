---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: 995f2cb41bf52b8992a2f6a8709177384a957a3d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35886173"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

boolean securityEnabledOnly = True;

graphClient.me()
    .getMemberObjects(securityEnabledOnly)
    .buildRequest()
    .post();

```