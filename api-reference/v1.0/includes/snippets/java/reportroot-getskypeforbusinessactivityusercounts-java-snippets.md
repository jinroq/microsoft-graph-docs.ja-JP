---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7f16ceafbceba5f7c039f8533f7346d39a82302e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892539"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getSkypeForBusinessActivityUserCounts('D7')
    .buildRequest()
    .get();

```