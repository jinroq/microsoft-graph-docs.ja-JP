---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c3d731c6d84e18f48f47d0273bd1854e0429b83b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320500"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getTeamsDeviceUsageUserCounts("D7")
    .buildRequest()
    .get();

```