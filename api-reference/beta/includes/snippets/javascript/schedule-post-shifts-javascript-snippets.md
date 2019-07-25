---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c44c1e892f4a7d729f37c72ba0cd2bf3a86673f6
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35718171"
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
    .post({shift : shift});

```