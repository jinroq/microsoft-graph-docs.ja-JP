---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: 3a4d745e6dd407f878c329ea37e6e81aa3ac6862
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35890972"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("format", "{format}"));

Stream Stream = graphClient.customRequest("/me/drive/items/{item-id}/content", Stream.class)
    .buildRequest( requestOptions )
    .get();

```