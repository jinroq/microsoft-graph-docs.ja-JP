---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c9766e067214a716c0518fc748c9f8d1f6adb109
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35860107"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("11021").assignments("19002").submissions("850f51b7").resources("f2387c3b-ec39-4bf2-a399-d7242677f024")
    .buildRequest()
    .delete();

```