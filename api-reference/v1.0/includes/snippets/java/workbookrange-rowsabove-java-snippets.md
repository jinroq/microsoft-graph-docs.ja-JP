---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6f81d1ce49df0222c7c2dea35f05ed306a414a9f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35884985"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().root().workbook().worksheets("{id}")
    .range()
    .rowsAbove(count)
    .buildRequest()
    .post();

```