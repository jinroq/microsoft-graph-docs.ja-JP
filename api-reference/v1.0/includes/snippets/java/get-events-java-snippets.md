---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: 8245184ec6a28e36bdee90fcf142595eec1734f2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888873"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "outlook.timezone=\"Pacific Standard Time\""));

IEventCollectionPage events = graphClient.me().events()
    .buildRequest( requestOptions )
    .select("subject,body,bodyPreview,organizer,attendees,start,end,location")
    .get();

```