---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ece897dacc14004b505a6438f0d46cd8baa3a301
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36637900"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const shift = {
  id: "SHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8",
  userId: "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  schedulingGroupId: "TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
  sharedShift: {
    displayName: "Day shift",
    notes: "Please do inventory as part of your shift.",
    startDateTime: "2019-03-11T15:00:00Z",
    endDateTime: "2019-03-12T00:00:00Z",
    theme: "blue",
    activities: [
      {
        isPaid: true,
        startDateTime: "2019-03-11T15:00:00Z",
        endDateTime: "2019-03-11T15:15:00Z",
        code: "",
        displayName: "Lunch"
      }
    ]
  },
  draftShift: {
    displayName: "Day shift",
    notes: "Please do inventory as part of your shift.",
    startDateTime: "2019-03-11T15:00:00Z",
    endDateTime: "2019-03-12T00:00:00Z",
    theme: "blue",
    activities: [
      {
        isPaid: true,
        startDateTime: "2019-03-11T15:00:00Z",
        endDateTime: "2019-03-11T15:30:00Z",
        code: "",
        displayName: "Lunch"
      }
    ]
  }
};

let res = await client.api('/teams/{teamId}/schedule/shifts')
    .version('beta')
    .post(shift);

```