---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e79afc336049b632fe8ef51ca9b0ad5b8a5c106c
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/11/2019
ms.locfileid: "36846123"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var timeOff = new TimeOff
{
    UserId = "c5d0c76b-80c4-481c-be50-923cd8d680a1",
    SharedTimeOff = new TimeOffItem
    {
        TimeOffReasonId = "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
        StartDateTime = DateTimeOffset.Parse("2019-03-11T07:00:00Z"),
        EndDateTime = DateTimeOffset.Parse("2019-03-12T07:00:00Z"),
        Theme = ScheduleEntityTheme.White
    },
    DraftTimeOff = new TimeOffItem
    {
        TimeOffReasonId = "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
        StartDateTime = DateTimeOffset.Parse("2019-03-11T07:00:00Z"),
        EndDateTime = DateTimeOffset.Parse("2019-03-12T07:00:00Z"),
        Theme = ScheduleEntityTheme.Pink
    }
};

await graphClient.Teams["{teamId}"].Schedule.TimesOff["{timeOffId}"]
    .Request()
    .Header("Prefer","return=representation")
    .PutAsync(timeOff);

```