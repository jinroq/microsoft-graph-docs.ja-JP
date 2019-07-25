---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6baa80e9ed4ca4ab9c118d20e276fd554a744cd9
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35708851"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var targets = new List<InvitationParticipantInfo>()
{
    new InvitationParticipantInfo
    {
        EndpointType = EndpointType.Default,
        Identity = new IdentitySet
        {
            User = new Identity
            {
                Id = "550fae72-d251-43ec-868c-373732c2704f",
                TenantId = "72f988bf-86f1-41af-91ab-2d7cd011db47",
                DisplayName = "Heidi Steen"
            }
        },
        LanguageId = "en-US",
        Region = "westus"
    }
};

var targetDisposition = CallDisposition.Default;

var timeout = 99;

var maskCallee = false;

var maskCaller = false;

await graphClient.App.Calls["{id}"]
    .Redirect(targets,targetDisposition,timeout,maskCallee,maskCaller)
    .Request()
    .PostAsync();

```