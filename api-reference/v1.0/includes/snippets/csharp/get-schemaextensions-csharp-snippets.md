---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8d5e88b8a65a35e21615eba492ad5cb6b6e5c1a2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35513875"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schemaExtensions = await graphClient.SchemaExtensions
    .Request()
    .Filter("id eq 'graphlearn_test'")
    .GetAsync();

```