---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: a2d6c54e0bec892cb0a45ba6abc4d67eb0be5f0d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35889146"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionPage memberOf = graphClient.groups("{id}").memberOf()
    .buildRequest()
    .get();

```