---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9169ed2044da5d6a4e1e359169b64088e85912a5
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875459"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Program program = new Program();
program.displayName = "testprogram3";
program.description = "test description";

graphClient.programs()
    .buildRequest()
    .post(program);

```