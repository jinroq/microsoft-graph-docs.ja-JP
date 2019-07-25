---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 494e5069def0ffb0e0bbe8905c86bd03347f9553
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35864987"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CalendarGroup calendarGroup = graphClient.me().calendarGroups("{id}")
    .buildRequest()
    .get();

```