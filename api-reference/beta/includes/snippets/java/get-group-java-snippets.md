---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a3e57772265f60e762ccb4469c7b78ed375d9001
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35858621"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Group group = graphClient.groups("45b7d2e7-b882-4a80-ba97-10b7a63b8fa4")
    .buildRequest()
    .get();

```