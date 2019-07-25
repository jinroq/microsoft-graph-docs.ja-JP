---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 235b7a0e8a8fa24c2dcc19fe790f44b7a4292abe
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35721012"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contacts = await graphClient.Contacts
    .Request()
    .GetAsync();

```