---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: 07fa812bea0da571892949e3b6f5f978a88adc99
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892810"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "odata.maxpagesize=2"));

IMessageDeltaCollectionPage delta = graphClient.me().mailFolders("{id}").messages()
    .delta()
    .buildRequest( requestOptions )
    .get();

```