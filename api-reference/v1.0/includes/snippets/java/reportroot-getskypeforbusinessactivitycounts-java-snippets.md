---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6c09bf81cf57ce61167755392780498acd846731
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35885924"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getSkypeForBusinessActivityCounts('D7')
    .buildRequest()
    .get();

```