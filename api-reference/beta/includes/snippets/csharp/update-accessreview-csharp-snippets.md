---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4afd13dfcfc245a698e55c900308872b7aee1e45
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35710907"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessReview = new AccessReview
{
    DisplayName = "TestReview new name"
};

await graphClient.AccessReviews["006111db-0810-4494-a6df-904d368bd81b"]
    .Request()
    .UpdateAsync(accessReview);

```