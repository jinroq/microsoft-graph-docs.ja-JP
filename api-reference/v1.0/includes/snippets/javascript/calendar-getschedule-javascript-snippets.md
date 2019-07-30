---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: b4364f592976b25538d08b30f21f392ff0040680
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932101"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const scheduleInformation = {
    schedules: ["adelev@contoso.onmicrosoft.com", "meganb@contoso.onmicrosoft.com"],
    startTime: {
        dateTime: "2019-03-15T09:00:00",
        timeZone: "Pacific Standard Time"
    },
    endTime: {
        dateTime: "2019-03-15T18:00:00",
        timeZone: "Pacific Standard Time"
    },
    availabilityViewInterval: "60"
};

let res = await client.api('/me/calendar/getschedule')
    .post(scheduleInformation);

```