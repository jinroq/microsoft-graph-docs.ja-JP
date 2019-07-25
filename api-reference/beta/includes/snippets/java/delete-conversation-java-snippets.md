---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 47f977e32a94fa05172c9699b24677758398b995
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35863041"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.groups("{id}").conversations("{id}")
    .buildRequest()
    .delete();

```