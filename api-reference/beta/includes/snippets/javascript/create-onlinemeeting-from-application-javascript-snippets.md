---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 59747d0f9db174a15bdf57cbae6ec3adee872ba9
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35711481"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const OnlineMeeting = {
  meetingType: "meetNow",
  participants: {
    organizer: {
      identity: {
        user: {
          id: "550fae72-d251-43ec-868c-373732c2704f"
        }
      }
    }
  },
  subject: "subject-value"
};

let res = await client.api('/app/onlineMeetings')
    .version('beta')
    .post({OnlineMeeting : OnlineMeeting});

```