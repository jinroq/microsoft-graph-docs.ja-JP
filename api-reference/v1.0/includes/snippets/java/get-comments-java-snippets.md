---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d0fced68879d4ecd37f14cc5a69f3b94b7c6454c
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/11/2019
ms.locfileid: "36839120"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IWorkbookCommentCollectionPage comments = graphClient.drive().root().workbook().comments()
    .buildRequest()
    .get();

```