---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fea6aae18560481ffe2c517900813c7c4f852182
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371626"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getOneDriveUsageAccountDetail("D7")
    .buildRequest()
    .get();

```