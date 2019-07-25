---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8e719a960c8246382dd2c9527d3ecdfeb6125e10
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35879288"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookNamedItem workbookNamedItem = graphClient.me().drive().items("{id}").workbook().names("{name}")
    .buildRequest()
    .get();

```