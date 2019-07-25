---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6a0f7000a064b61f991814d408367780d387d7f6
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893959"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getOffice365GroupsActivityDetail('D7')
    .buildRequest()
    .get();

```