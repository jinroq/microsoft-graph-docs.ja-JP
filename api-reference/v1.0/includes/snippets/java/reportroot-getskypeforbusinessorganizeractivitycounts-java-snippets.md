---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 64b48757272acf443bdac8380427e9c1122a43e8
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892374"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getSkypeForBusinessOrganizerActivityCounts('D7')
    .buildRequest()
    .get();

```