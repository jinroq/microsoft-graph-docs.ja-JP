---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: 1eb016705c68e0b4fcbd04b23dac300d6ef806fa
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881649"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDriveItemCollectionPage search = graphClient.me().drive().root()
    .search('{search-query}')
    .buildRequest()
    .get();

```