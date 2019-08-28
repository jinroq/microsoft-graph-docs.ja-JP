---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b100c9015892f148dbb89b55aa724d52c1785b4e
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36637852"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const onlineMeeting = {
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
    .post(onlineMeeting);

```