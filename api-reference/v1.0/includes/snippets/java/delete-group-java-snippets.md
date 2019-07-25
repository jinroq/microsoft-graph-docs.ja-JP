---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a27f251232fe3f8cac26da65b54d78ba0caa06fa
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35890714"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.groups("{id}")
    .buildRequest()
    .delete();

```