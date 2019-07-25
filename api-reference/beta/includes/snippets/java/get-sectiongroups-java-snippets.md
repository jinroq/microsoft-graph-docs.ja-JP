---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b2fc32ea3c8664846ec0f4f975effb12ce69b036
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35870482"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISectionGroupCollectionPage sectionGroups = graphClient.me().onenote().sectionGroups("{id}").sectionGroups()
    .buildRequest()
    .get();

```