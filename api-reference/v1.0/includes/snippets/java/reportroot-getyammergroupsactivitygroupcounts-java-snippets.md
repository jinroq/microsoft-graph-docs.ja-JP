---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9414d81f993bb0856cf51d7b1ca5db05d1ab5522
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36347685"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getYammerGroupsActivityGroupCounts("D7")
    .buildRequest()
    .get();

```