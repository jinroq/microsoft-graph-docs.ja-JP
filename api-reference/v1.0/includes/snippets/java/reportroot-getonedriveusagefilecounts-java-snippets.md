---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3731b97c103bcb403925e641646592619c9fb38e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36321892"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getOneDriveUsageFileCounts("D7")
    .buildRequest()
    .get();

```