---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: edab56fb2fdfa6d2dd8f671fe866cb6bc412547a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867871"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("ba9a3254-9f18-4209-aeb3-9e42a35b5be4")
    .buildRequest()
    .delete();

```