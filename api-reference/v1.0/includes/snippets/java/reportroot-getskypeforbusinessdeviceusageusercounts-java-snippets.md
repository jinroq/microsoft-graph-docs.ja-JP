---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5a39d60cde84a7d89b55b3f124cf573b3faa3ad6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349292"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getSkypeForBusinessDeviceUsageUserCounts("D7")
    .buildRequest()
    .get();

```