---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: a2af1ddf11c82c964bb50a64a525de6714f7bc4d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881186"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "odata.maxpagesize=2"));
requestOptions.add(new QueryOption("startdatetime", "2016-12-01T00:00:00Z"));
requestOptions.add(new QueryOption("enddatetime", "2016-12-30T00:00:00Z"));

IEventDeltaCollectionPage delta = graphClient.me().calendarView()
    .delta()
    .buildRequest( requestOptions )
    .get();

```