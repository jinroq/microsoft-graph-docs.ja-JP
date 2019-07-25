---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 61c7986b8c3b4d371482dc2ab353322a59916cf6
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881002"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemReference parentReference = new ItemReference();
parentReference.path = "/drive/root:/Documents";

String name = "Copy of LargeFolder1";

graphClient.me().drive().items("{folder-item-id}")
    .copy(name,parentReference)
    .buildRequest()
    .post();

```