---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: cd42b43e4319ddff687a0ff50d69ddd863bd9c8c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891671"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeSort workbookRangeSort = graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range().sort()
    .buildRequest()
    .get();

```