---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: df0542a77e97d0eb0c72094e26f8226b0df554e4
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359845"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISharePointActivityUserCountsCollectionPage getSharePointActivityUserCounts = graphClient.reports()
    .getSharePointActivityUserCounts("D7")
    .buildRequest()
    .get();

```