---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e618f39671ae0c1decea649717e0b495822abe1d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34465595"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingStaffMember = new BookingStaffMember
{
    WorkingHours = new List<BookingWorkHours>()
    {
        new BookingWorkHours
        {
            Day = DayOfWeek.Monday,
            TimeSlots = new List<BookingWorkTimeSlot>()
            {
            }
        },
        new BookingWorkHours
        {
            Day = DayOfWeek.Tuesday,
            TimeSlots = new List<BookingWorkTimeSlot>()
            {
                new BookingWorkTimeSlot
                {
                    End = "17:00:00.0000000",
                    Start = "08:00:00.0000000"
                }
            }
        },
        new BookingWorkHours
        {
            Day = DayOfWeek.Wednesday,
            TimeSlots = new List<BookingWorkTimeSlot>()
            {
                new BookingWorkTimeSlot
                {
                    End = "17:00:00.0000000",
                    Start = "08:00:00.0000000"
                }
            }
        },
        new BookingWorkHours
        {
            Day = DayOfWeek.Thursday,
            TimeSlots = new List<BookingWorkTimeSlot>()
            {
                new BookingWorkTimeSlot
                {
                    End = "17:00:00.0000000",
                    Start = "08:00:00.0000000"
                }
            }
        },
        new BookingWorkHours
        {
            Day = DayOfWeek.Friday,
            TimeSlots = new List<BookingWorkTimeSlot>()
            {
                new BookingWorkTimeSlot
                {
                    End = "17:00:00.0000000",
                    Start = "08:00:00.0000000"
                }
            }
        }
    }
};

await graphClient.BookingBusinesses["Contosolunchdelivery@M365B489948.onmicrosoft.com"].StaffMembers["8ee1c803-a1fa-406d-8259-7ab53233f148"]
    .Request()
    .UpdateAsync(bookingStaffMember);

```