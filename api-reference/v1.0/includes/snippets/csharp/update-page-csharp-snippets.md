---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5bf168a4f16b9c3bf06af4699d03846ab8659366
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35495686"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var Stream = new List<Stream>()
{
    new Stream
    {
        Target = "#para-id",
        Action = "insert",
        Position = "before",
        Content = "<img src=\"image-url-or-part-name\" alt=\"image-alt-text\" />"
    },
    new Stream
    {
        Target = "#list-id",
        Action = "append",
        Content = "<li>new-page-content</li>"
    }
};

var pages = new OnenotePage();
pages.Content = content;

await graphClient.Me.Onenote.Pages["{id}"]
    .Request()
    .UpdateAsync(pages);

```