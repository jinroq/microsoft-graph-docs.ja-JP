---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 35d6f596cca6d55fdc702636e274ef229325d31f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35862456"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("$filter", "isOf('Microsoft.Graph.User')+or+isOf('Microsoft.Graph.Group')"));

DirectoryObject directoryObject = graphClient.directoryObjects("delta")
    .buildRequest( requestOptions )
    .get();

```