---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: f53ddc3bc804724d6201bf1ceab8a4bd0b69a43c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891034"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDriveItemDeltaCollectionPage delta = graphClient.me().drive().root()
    .delta('1230919asd190410jlka')
    .buildRequest()
    .get();

```