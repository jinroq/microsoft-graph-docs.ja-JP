---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 66b832600d7ce9a27d5b882ce3de47b86bb2e3e4
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932865"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = new DriveItem
{
    Name = "My Day at the Beach",
    @name.conflictBehavior = "rename",
    Bundle = new Bundle
    {
        Album = new Album
        {
        }
    },
    Children = new List<DriveItem>()
    {
        new DriveItem
        {
            Id = "1234asdf"
        }
    }
};

await graphClient.Drive.Bundles
    .Request()
    .AddAsync(driveItem);

```