---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c755a12cc2a58b389df229f0b2cad34acc2ff224
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/11/2019
ms.locfileid: "36839155"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookComment workbookComment = graphClient.drive().root().workbook().comments("{id}")
    .buildRequest()
    .get();

```