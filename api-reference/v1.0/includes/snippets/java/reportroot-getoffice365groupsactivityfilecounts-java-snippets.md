---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 66efae40393531d0920a28eb3359c78e51bb860f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36373725"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getOffice365GroupsActivityFileCounts("D7")
    .buildRequest()
    .get();

```