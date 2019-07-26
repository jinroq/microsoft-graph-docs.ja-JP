---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: 1162eae62a9404c1fbfc7f3d8102621a56b29ef5
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888876"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IGroupCollectionPage joinedTeams = graphClient.me().joinedTeams()
    .buildRequest()
    .get();

```