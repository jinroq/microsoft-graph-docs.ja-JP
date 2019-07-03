---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0a963a9d109ec1a15bfb2061967fd76a0df6b0a3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35495918"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contacts = await graphClient.Me.Contacts
    .Request()
    .GetAsync();

```