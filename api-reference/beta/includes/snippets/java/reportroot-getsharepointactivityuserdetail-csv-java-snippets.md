---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: cdae176cfcc204d2e7390b6a36b9603961972877
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359949"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISharePointActivityUserDetailCollectionPage getSharePointActivityUserDetail = graphClient.reports()
    .getSharePointActivityUserDetail("D7")
    .buildRequest()
    .get();

```