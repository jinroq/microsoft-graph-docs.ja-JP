---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 88db1d5a77479fe5bf4b3dcfe0999902f403c7b9
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36374002"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getOneDriveActivityFileCounts("D7")
    .buildRequest()
    .get();

```