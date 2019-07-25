---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9b8fde04c45a421639c98901ffcf7b742d9fe393
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724395"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var addLicenses = new List<AssignedLicense>()
{
    new AssignedLicense
    {
        DisabledPlans = new List<String>()
        {
            "11b0131d-43c8-4bbb-b2c8-e80f9a50834a"
        },
        SkuId = "skuId-value-1"
    },
    new AssignedLicense
    {
        DisabledPlans = new List<String>()
        {
            "a571ebcc-fqe0-4ca2-8c8c-7a284fd6c235"
        },
        SkuId = "skuId-value-2"
    }
};

var removeLicenses = new List<String>()
{
};

await graphClient.Me
    .AssignLicense(addLicenses,removeLicenses)
    .Request()
    .PostAsync();

```