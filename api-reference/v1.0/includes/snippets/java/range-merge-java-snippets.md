---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5b717e5df5052255bf1b0e7a02eb3d31c5ecfae4
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891302"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

boolean across = True;

graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range()
    .merge(across)
    .buildRequest()
    .post();

```