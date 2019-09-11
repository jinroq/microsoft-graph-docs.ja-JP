---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a94f1f003d1eed9f407cbb104d36c7ff57e002ec
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/11/2019
ms.locfileid: "36838774"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var call = new Call
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.type","#microsoft.graph.call"}
    },
    CallbackUri = "https://bot.contoso.com/callback",
    Targets = new List<ParticipantInfo>()
    {
        new ParticipantInfo
        {
            AdditionalData = new Dictionary<string, object>()
            {
                {"@odata.type","#microsoft.graph.participantInfo"}
            },
            Identity = new IdentitySet
            {
                AdditionalData = new Dictionary<string, object>()
                {
                    {"@odata.type","#microsoft.graph.identitySet"}
                },
                User = new Identity
                {
                    AdditionalData = new Dictionary<string, object>()
                    {
                        {"@odata.type","#microsoft.graph.identity"}
                    },
                    DisplayName = "John",
                    Id = "112f7296-5fa4-42ca-bae8-6a692b15d4b8"
                }
            }
        }
    },
    RequestedModalities = new List<Modality>()
    {
        Modality.Audio
    },
    MediaConfig = new MediaConfig
    {
        AdditionalData = new Dictionary<string, object>()
        {
            {"@odata.type","#microsoft.graph.serviceHostedMediaConfig"}
        }
    }
};

await graphClient.App.Calls
    .Request()
    .Header("Authorization","Bearer <Token>")
    .AddAsync(call);

```