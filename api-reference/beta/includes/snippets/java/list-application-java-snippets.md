---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: f0304ed0a2a082e8f3cb9176c1d68c48aa5994c3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855237"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IApplicationCollectionPage applications = graphClient.applications()
    .buildRequest()
    .get();

```