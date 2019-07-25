---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2ae96e5fdfca2b7b91bffbe776554d5cc4dd7ab4
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35862565"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IGroupCollectionPage microsoft.graph.group = graphClient.directory().deletedItems().microsoft.graph.group()
    .buildRequest()
    .get();

```