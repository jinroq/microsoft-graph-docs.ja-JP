---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7ef0433d1fadb602c1466f87e7310e5c7879fde7
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35883023"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOnenoteSectionCollectionPage sections = graphClient.me().onenote().sectionGroups("{id}").sections()
    .buildRequest()
    .get();

```