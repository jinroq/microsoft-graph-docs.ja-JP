---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d8a312e19299ed43c7d1162777a2dfe5f12004eb
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359488"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISkypeForBusinessDeviceUsageUserCountsCollectionPage getSkypeForBusinessDeviceUsageUserCounts = graphClient.reports()
    .getSkypeForBusinessDeviceUsageUserCounts("D7")
    .buildRequest()
    .get();

```