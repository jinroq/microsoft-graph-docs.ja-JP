---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: e70fe49ce7023e08b8c08267d12bf856d9ccd366
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881185"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "odata.maxpagesize=2"));

IEventDeltaCollectionPage delta = graphClient.me().calendarView()
    .delta()
    .buildRequest( requestOptions )
    .get();

```