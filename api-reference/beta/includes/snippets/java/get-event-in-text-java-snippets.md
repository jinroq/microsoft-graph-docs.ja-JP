---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a192cd1654df33c9959ce2207bea1f653217cf48
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35859632"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "outlook.body-content-type=\"text\""));

Event event = graphClient.me().events("AAMkAGI1AAAoZDOFAAA=")
    .buildRequest( requestOptions )
    .select("subject,body,bodyPreview")
    .get();

```