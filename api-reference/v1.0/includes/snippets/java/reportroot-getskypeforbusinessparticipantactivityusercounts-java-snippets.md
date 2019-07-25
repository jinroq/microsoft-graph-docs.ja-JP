---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6ce221cab33f20d1914111f68d2101fde08e7145
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892294"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getSkypeForBusinessParticipantActivityUserCounts('D7')
    .buildRequest()
    .get();

```