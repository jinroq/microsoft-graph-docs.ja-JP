---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d4d54cae9fa3bb88838f4037a114ea08e5b6239a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36374399"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getOffice365ServicesUserCounts("D7")
    .buildRequest()
    .get();

```