---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4cf835822f64642d73831ec5be002d360b4ac2dd
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36360196"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOneDriveActivityUserDetailCollectionPage getOneDriveActivityUserDetail = graphClient.reports()
    .getOneDriveActivityUserDetail("D7")
    .buildRequest()
    .get();

```