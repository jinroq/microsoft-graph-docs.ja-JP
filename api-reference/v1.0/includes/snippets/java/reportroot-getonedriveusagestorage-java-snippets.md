---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 394670a3fbc87a7b1f2416f5701f5927bccb10c7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36321871"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getOneDriveUsageStorage("D7")
    .buildRequest()
    .get();

```