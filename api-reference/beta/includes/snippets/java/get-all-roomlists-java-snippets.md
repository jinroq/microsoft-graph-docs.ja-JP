---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3a1738e96eb89120cd33cb01ba928a70a4eeec5a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35876790"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IRoomListCollectionPage microsoft.graph.roomlist = graphClient.places().microsoft.graph.roomlist()
    .buildRequest()
    .get();

```