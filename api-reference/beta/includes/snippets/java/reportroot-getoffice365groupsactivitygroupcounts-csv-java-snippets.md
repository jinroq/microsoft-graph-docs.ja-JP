---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9a37b0afd46e881f861f04fa38001cd159dc4569
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36360405"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOffice365GroupsActivityGroupCountsCollectionPage getOffice365GroupsActivityGroupCounts = graphClient.reports()
    .getOffice365GroupsActivityGroupCounts("D7")
    .buildRequest()
    .get();

```