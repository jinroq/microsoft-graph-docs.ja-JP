---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 27480439678af338071374f883eea816100c3d94
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35861199"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("format", "{format}"));

Stream Stream = graphClient.customRequest("/drive/items/{item-id}/content", Stream.class)
    .buildRequest( requestOptions )
    .get();

```