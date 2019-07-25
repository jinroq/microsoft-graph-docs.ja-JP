---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4f3c983e1d1bf1196f80be53670c3a91847674b7
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35890280"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range()
    .buildRequest()
    .post();

```