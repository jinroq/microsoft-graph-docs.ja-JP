---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6a337b4033b69e25beb5afaa10aa4fd86e3adfce
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35860736"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("11021").assignments("19002").resources("22002")
    .buildRequest()
    .delete();

```