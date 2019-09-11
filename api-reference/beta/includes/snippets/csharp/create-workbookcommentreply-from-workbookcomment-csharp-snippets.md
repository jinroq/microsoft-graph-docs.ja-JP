---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c83fd55e400da437ead3aa2f685cc0d30c5e1224
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/11/2019
ms.locfileid: "36838928"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookCommentReply = new WorkbookCommentReply
{
    Content = "This is my reply to the comment.",
    ContentType = "plain"
};

await graphClient.Drive.Root.Workbook.Comments["{id}"].Replies
    .Request()
    .AddAsync(workbookCommentReply);

```