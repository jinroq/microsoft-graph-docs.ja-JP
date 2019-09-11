---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6dbd360c41743a1f8edb6e74730c47af86c39fdf
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/11/2019
ms.locfileid: "36839010"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookCommentReply workbookCommentReply = graphClient.drive().root().workbook().comments("{id}").replies("{id}")
    .buildRequest()
    .get();

```